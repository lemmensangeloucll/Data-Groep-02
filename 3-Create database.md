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
CREATE TABLE IF NOT EXISTS klanten (
  id INT NOT NULL,
  voornaam text NOT NULL,
  achternaam text NOT NULL,
  straatnaam text NOT NULL,
  huisnummer text NOT NULL,
  gemeente text NOT NULL,
  postcode text NOT NULL,
  PRIMARY KEY (id)
  );
grant all on table klanten TO "r0797739";
grant all on table klanten TO "r0753029";
grant all on table klanten TO "r0795520";

CREATE TABLE IF NOT EXISTS bungalowpark (
  id INT NOT NULL,
  straat text NULL,
  huisnummer text NULL,
  postcode text NULL,
  gemeente text NULL,
  PRIMARY KEY (id)
  );
grant all on table bungalowpark TO "r0797739";
grant all on table bungalowpark TO "r0753029";
grant all on table bungalowpark TO "r0795520";

CREATE TABLE IF NOT EXISTS periode (
  id INT NOT NULL,
  duur text NULL,
  datum date NULL,
  seizoen text NULL,
  PRIMARY KEY (id)
  );
grant all on table periode TO "r0797739";
grant all on table periode TO "r0753029";
grant all on table periode TO "r0795520";

CREATE TABLE IF NOT EXISTS bungalowtype (
  id INT NOT NULL,
  klasse text NULL,
  capaciteit INT NULL,
  PRIMARY KEY (id)
  );
grant all on table bungalowtype TO "r0797739";
grant all on table bungalowtype TO "r0753029";
grant all on table bungalowtype TO "r0795520";

CREATE TABLE IF NOT EXISTS zone (
  id INT NOT NULL,
  uitzicht text NULL,
  nabijheid text NULL,
  PRIMARY KEY (id)
  );
grant all on table zone TO "r0797739";
grant all on table zone TO "r0753029";
grant all on table zone TO "r0795520";

CREATE TABLE IF NOT EXISTS bungalow (
  bungalownummer INT NOT NULL,
  ontruimd text NULL,
  beschikbaarheid text NULL,
  bungalowtype INT NOT NULL,
  bungalowpark INT NOT NULL,
  zone INT NOT NULL,
  PRIMARY KEY (bungalownummer, bungalowtype, bungalowpark, zone),
  CONSTRAINT fk_bungalow_bungalowtype1
    FOREIGN KEY (bungalowtype)
    REFERENCES R1TX32_team02.bungalowtype (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_bungalow_bungalowpark1
    FOREIGN KEY (bungalowpark)
    REFERENCES R1TX32_team02.bungalowpark (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_bungalow_zone1
    FOREIGN KEY (zone)
    REFERENCES R1TX32_team02.zone (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION
    );
grant all on table bungalow TO "r0797739";
grant all on table bungalow TO "r0753029";
grant all on table bungalow TO "r0795520";

CREATE TABLE IF NOT EXISTS reservaties (
  reservatienummer INT NOT NULL DEFAULT NEXTVAL ('R1TX32_team02.reservaties_seq'),
  contacttype text NOT NULL,
  datum date NOT NULL DEFAULT current_timestamp(),
  annulatieverzekering SMALLINT NULL,
  bungalowpark INT NOT NULL,
  periode INT NOT NULL,
  bungalowtype INT NOT NULL,
  klant INT NOT NULL,
  bungalow INT NOT NULL,
  res_status text NULL DEFAULT 'aanvraag',
  PRIMARY KEY (reservatienummer, bungalowpark, periode, bungalowtype, klant, bungalow),
  CONSTRAINT fk_reservaties_bungalowpark1
    FOREIGN KEY (bungalowpark)
    REFERENCES R1TX32_team02.bungalowpark (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_periode1
    FOREIGN KEY (periode)
    REFERENCES R1TX32_team02.periode (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_bungalowtype1
    FOREIGN KEY (bungalowtype)
    REFERENCES R1TX32_team02.bungalowtype (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_klanten1
    FOREIGN KEY (klant)
    REFERENCES R1TX32_team02.klanten (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_bungalow1
    FOREIGN KEY (bungalow)
    REFERENCES R1TX32_team02.bungalow (bungalownummer)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION
    );
grant all on table reservaties TO "r0797739";
grant all on table reservaties TO "r0753029";
grant all on table reservaties TO "r0795520";

CREATE TABLE IF NOT EXISTS arrangement (
  id INT NOT NULL,
  diensten text NULL,
  bijkomende prijs DECIMAL(6,2) NULL,
  activiteiten text NULL,
  PRIMARY KEY (id)
  );
grant all on table arrangement TO "r0797739";
grant all on table arrangement TO "r0753029";
grant all on table arrangement TO "r0795520";
  
CREATE TABLE IF NOT EXISTS faciliteiten (
  id INT NOT NULL,
  faciliteit text NULL,
  PRIMARY KEY (id)
  );
grant all on table faciliteiten TO "r0797739";
grant all on table faciliteiten TO "r0753029";
grant all on table faciliteiten TO "r0795520";

CREATE TABLE IF NOT EXISTS bungalowtype_has_faciliteiten (
  bungalowtype INT NOT NULL,
  faciliteit INT NOT NULL,
  PRIMARY KEY (bungalowtype, faciliteit),
  CONSTRAINT fk_bungalowtype_has_faciliteiten_bungalowtype
    FOREIGN KEY (bungalowtype)
    REFERENCES R1TX32_team02.bungalowtype (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_bungalowtype_has_faciliteiten_faciliteiten1
    FOREIGN KEY (faciliteit)
    REFERENCES R1TX32_team02.faciliteiten (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION
    );
grant all on table bungalowtype_has_faciliteiten TO "r0797739";
grant all on table bungalowtype_has_faciliteiten TO "r0753029";
grant all on table bungalowtype_has_faciliteiten TO "r0795520";

CREATE TABLE IF NOT EXISTS facturen (
  id INT NOT NULL,
  factuurnummer text NULL,
  beschrijving text NULL,
  prijs DECIMAL(10,2) NULL,
  btw DECIMAL(10,2) NULL,
  korting DECIMAL(10,2) NULL,
  totale_prijs DECIMAL(20,2) NULL,
  klant INT NOT NULL,
  PRIMARY KEY (id, klant),
  CONSTRAINT fk_facturen_klanten1
    FOREIGN KEY (klant)
    REFERENCES R1TX32_team02.klanten (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION
    );
grant all on table facturen TO "r0797739";
grant all on table facturen TO "r0753029";
grant all on table facturen TO "r0795520";

CREATE TABLE IF NOT EXISTS reparatie_aanvragen (
  aanvraagnummer INT NOT NULL,
  tijdstip date NULL,
  prioriteit text NULL,
  beschrijving text NULL,
  vaardigheid text NULL,
  klant INT NOT NULL,
  bungalow INT NOT NULL,
  PRIMARY KEY (aanvraagnummer, bungalow),
  CONSTRAINT fk_reparatie_aanvragen_klanten1
    FOREIGN KEY (klant)
    REFERENCES R1TX32_team02.klanten (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reparatie_aanvragen_bungalow1
    FOREIGN KEY (bungalow)
    REFERENCES R1TX32_team02.bungalow (bungalownummer)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION
    );
grant all on table reparatie_aanvragen TO "r0797739";
grant all on table reparatie_aanvragen TO "r0753029";
grant all on table reparatie_aanvragen TO "r0795520";

CREATE TABLE IF NOT EXISTS reservaties_has_zone (
  reservatie INT NOT NULL,
  zone INT NOT NULL,
  prijs DECIMAL(10,2) NULL,
  PRIMARY KEY (reservatie, zone),
  CONSTRAINT fk_reservaties_has_zone_reservaties1
    FOREIGN KEY (reservatie)
    REFERENCES R1TX32_team02.reservaties (reservatienummer)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_has_zone_zone1
    FOREIGN KEY (zone)
    REFERENCES R1TX32_team02.zone (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION
    );
grant all on table reservaties_has_zone TO "r0797739";
grant all on table reservaties_has_zone TO "r0753029";
grant all on table reservaties_has_zone TO "r0795520";

CREATE TABLE IF NOT EXISTS reservaties_has_arrangement (
  reservatie INT NOT NULL,
  arrangement INT NOT NULL,
  PRIMARY KEY (reservatie, arrangement),
  CONSTRAINT fk_reservaties_has_arrangement_reservaties1
    FOREIGN KEY (reservatie)
    REFERENCES R1TX32_team02.reservaties (reservatienummer)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION,
  CONSTRAINT fk_reservaties_has_arrangement_arrangement1
    FOREIGN KEY (arrangement)
    REFERENCES R1TX32_team02.arrangement (id)
    ON DELETE NO ACTION
    ON UPDATE NO ACTION
    );
grant all on table reservaties_has_arrangement TO "r0797739";
grant all on table reservaties_has_arrangement TO "r0753029";
grant all on table reservaties_has_arrangement TO "r0795520";
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4MTIwMDI3NjAsOTk5OTE1OTcxLDIwOD
E4NTM2MzUsMTg3NzM5MTkxOV19
-->