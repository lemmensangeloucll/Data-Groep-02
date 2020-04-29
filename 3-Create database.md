## Create database

### Het aanmaken van het schema binnen de databank groepswerk
```
CREATE SCHEMA R1TX32_team02;
grant all on schema "R1TX32_team02" TO "r0797739";
grant all on schema "R1TX32_team02" TO "r0753029";
grant all on schema "R1TX32_team02" TO "r0795520";
```
### Het instellen van het correcte search path
```
SET search_path TO "R1TX32_team02";
```
 > TIP!
Als je een CREATE TABLE statement toevoegt in je CREATE script (na testen van dit statement), voeg dan ineens ook de DROP TABLE statement vooraan toe in je DROP script. 
Zo ben je zeker dat de volgorde correct is. 
Als je dan iets wil aanpassen in een tabel, pas dan ineens aan in het CREATE script en laat dan eerst het DROP script runnen en het volledige CREATE script. Zo ben je ook zeker dat er zich geen fouten voordoen (of kan je ze onmiddellijk oplossen)

### Aanmaken van de tabellen

> Run onderstaande code elke keer wanneer je een aanpassing gedaan hebt. 
> Hierna run je ook de inserts opnieuw.
```
CREATE TABLE klanten (
  id INT NOT NULL,
  voornaam text NOT NULL,
  achternaam text NOT NULL,
  straatnaam text NOT NULL,
  huisnummer text NOT NULL,
  gemeente text NOT NULL,
  postcode text NOT NULL,
  CONSTRAINT pk_klanten PRIMARY KEY (id)
  );
grant all on table klanten TO "r0797739";
grant all on table klanten TO "r0753029";
grant all on table klanten TO "r0795520";

CREATE TABLE bungalowpark (
  id INT NOT NULL,
  straat text NULL,
  huisnummer text NULL,
  postcode text NULL,
  gemeente text NULL,
  CONSTRAINT pk_bungalowpark PRIMARY KEY (id)
  );
grant all on table bungalowpark TO "r0797739";
grant all on table bungalowpark TO "r0753029";
grant all on table bungalowpark TO "r0795520";

CREATE TABLE periode (
  id INT NOT NULL,
  duur text NULL,
  datum date NULL,
  seizoen text NULL,
  CONSTRAINT pk_periode PRIMARY KEY (id)
  );
grant all on table periode TO "r0797739";
grant all on table periode TO "r0753029";
grant all on table periode TO "r0795520";

CREATE TABLE bungalowtype (
  id INT NOT NULL,
  klasse text NULL,
  capaciteit INT NULL,
  CONSTRAINT pk_bungalowtype PRIMARY KEY (id)
  );
grant all on table bungalowtype TO "r0797739";
grant all on table bungalowtype TO "r0753029";
grant all on table bungalowtype TO "r0795520";

CREATE TABLE zone (
  id INT NOT NULL,
  uitzicht text NULL,
  nabijheid text NULL,
  CONSTRAINT pk_zone PRIMARY KEY (id)
  );
grant all on table zone TO "r0797739";
grant all on table zone TO "r0753029";
grant all on table zone TO "r0795520";

CREATE TABLE bungalow (
  bungalownummer INT NOT NULL,
  ontruimd text NULL,
  beschikbaarheid text NULL,
  bungalowtype INT NOT NULL,
  bungalowpark INT NOT NULL,
  zone INT NOT NULL,
  CONSTRAINT pk_bungalow PRIMARY KEY (bungalownummer, bungalowpark),
  CONSTRAINT fk_bungalow_bungalowtype1
    FOREIGN KEY (bungalowtype)
    REFERENCES bungalowtype (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_bungalow_bungalowpark1
    FOREIGN KEY (bungalowpark)
    REFERENCES bungalowpark (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_bungalow_zone1
    FOREIGN KEY (zone)
    REFERENCES zone (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION
    );
grant all on table bungalow TO "r0797739";
grant all on table bungalow TO "r0753029";
grant all on table bungalow TO "r0795520";

CREATE TABLE reservaties (
  reservatienummer INT NOT NULL,
  contacttype text NOT NULL,
  datum date NOT NULL,
  annulatieverzekering SMALLINT NULL,
  bungalowpark INT NOT NULL,
  periode INT NOT NULL,
  bungalowtype INT NOT NULL,
  klant INT NOT NULL,
  bungalow INT NOT NULL,
  res_status text NULL DEFAULT 'aanvraag',
  CONSTRAINT pk_reservaties PRIMARY KEY (reservatienummer),
  CONSTRAINT fk_reservaties_bungalowpark1
    FOREIGN KEY (bungalowpark)
    REFERENCES bungalowpark (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_periode1
    FOREIGN KEY (periode)
    REFERENCES periode (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_bungalowtype1
    FOREIGN KEY (bungalowtype)
    REFERENCES bungalowtype (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_klanten1
    FOREIGN KEY (klant)
    REFERENCES klanten (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_bungalow1
    FOREIGN KEY (bungalow, bungalowpark)
    REFERENCES bungalow (bungalownummer, bungalowpark)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION
    );
grant all on table reservaties TO "r0797739";
grant all on table reservaties TO "r0753029";
grant all on table reservaties TO "r0795520";

CREATE TABLE arrangement (
  id INT NOT NULL,
  diensten text NULL,
  bijkomende_prijs DECIMAL(6,2) NULL,
  activiteiten text NULL,
  CONSTRAINT pk_arrangement PRIMARY KEY (id),
  CONSTRAINT check_prijs CHECK(bijkomende_prijs > 0)
  );
grant all on table arrangement TO "r0797739";
grant all on table arrangement TO "r0753029";
grant all on table arrangement TO "r0795520";
  
CREATE TABLE faciliteiten (
  id INT NOT NULL,
  faciliteit text NULL,
  CONSTRAINT pk_faciliteiten PRIMARY KEY (id)
  );
grant all on table faciliteiten TO "r0797739";
grant all on table faciliteiten TO "r0753029";
grant all on table faciliteiten TO "r0795520";

CREATE TABLE bungalowtype_has_faciliteiten (
  bungalowtype INT NOT NULL,
  faciliteit INT NOT NULL,
  CONSTRAINT pk_bungalowtype_has_faciliteiten PRIMARY KEY (bungalowtype, faciliteit),
  CONSTRAINT fk_bungalowtype_has_faciliteiten_bungalowtype
    FOREIGN KEY (bungalowtype)
    REFERENCES bungalowtype (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_bungalowtype_has_faciliteiten_faciliteiten1
    FOREIGN KEY (faciliteit)
    REFERENCES faciliteiten (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION
    );
grant all on table bungalowtype_has_faciliteiten TO "r0797739";
grant all on table bungalowtype_has_faciliteiten TO "r0753029";
grant all on table bungalowtype_has_faciliteiten TO "r0795520";

CREATE TABLE facturen (
  id INT NOT NULL,
  factuurnummer text NULL,
  beschrijving text NULL,
  prijs DECIMAL(10,2) NULL,
  btw DECIMAL(10,2) NULL,
  korting DECIMAL(10,2) NULL,
  totale_prijs DECIMAL(20,2) NULL,
  klant INT NOT NULL,
  CONSTRAINT fk_facturen PRIMARY KEY (id, klant),
  CONSTRAINT fk_facturen_klanten1
    FOREIGN KEY (klant)
    REFERENCES klanten (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION
    );
grant all on table facturen TO "r0797739";
grant all on table facturen TO "r0753029";
grant all on table facturen TO "r0795520";

CREATE TABLE reparatie_aanvragen (
  aanvraagnummer INT NOT NULL,
  tijdstip date NULL,
  prioriteit text NULL,
  beschrijving text NULL,
  vaardigheid text NULL,
  klant INT NOT NULL,
  bungalow INT NOT NULL,
  CONSTRAINT pk_reparatie_aanvragen PRIMARY KEY (aanvraagnummer, bungalow),
  CONSTRAINT fk_reparatie_aanvragen_klanten1
    FOREIGN KEY (klant)
    REFERENCES klanten (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reparatie_aanvragen_bungalow1
    FOREIGN KEY (bungalow)
    REFERENCES bungalow (bungalownummer)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION
    );
grant all on table reparatie_aanvragen TO "r0797739";
grant all on table reparatie_aanvragen TO "r0753029";
grant all on table reparatie_aanvragen TO "r0795520";

CREATE TABLE reservaties_has_zone (
  reservatie INT NOT NULL,
  zone INT NOT NULL,
  prijs DECIMAL(10,2) NULL,
  CONSTRAINT pk_reservatie_has_zone PRIMARY KEY (reservatie, zone),
  CONSTRAINT fk_reservaties_has_zone_reservaties1
    FOREIGN KEY (reservatie)
    REFERENCES reservaties (reservatienummer)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_has_zone_zone1
    FOREIGN KEY (zone)
    REFERENCES zone (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION
    );
grant all on table reservaties_has_zone TO "r0797739";
grant all on table reservaties_has_zone TO "r0753029";
grant all on table reservaties_has_zone TO "r0795520";

CREATE TABLE reservaties_has_arrangement (
  reservatie INT NOT NULL,
  arrangement INT NOT NULL,
  CONSTRAINT pk_reservaties_has_arrangement PRIMARY KEY (reservatie, arrangement),
  CONSTRAINT fk_reservaties_has_arrangement_reservaties1
    FOREIGN KEY (reservatie)
    REFERENCES reservaties (reservatienummer)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_has_arrangement_arrangement1
    FOREIGN KEY (arrangement)
    REFERENCES arrangement (id)
    ON DELETE RESTRICT
    ON UPDATE NO ACTION
    );
grant all on table reservaties_has_arrangement TO "r0797739";
grant all on table reservaties_has_arrangement TO "r0753029";
grant all on table reservaties_has_arrangement TO "r0795520";
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzIyMzYzODg5LDEwMzYyNzM2MjIsLTIxNz
U5ODUwMyw1NjM3MjgwNzMsLTE4MTIwMDI3NjAsOTk5OTE1OTcx
LDIwODE4NTM2MzUsMTg3NzM5MTkxOV19
-->