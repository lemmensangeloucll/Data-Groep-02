## Create database

### Het aanmaken van het schema binnen de databank groepswerk
```
CREATE SCHEMA R1TX32_team02;
grant all on schema "R1TX32_team02" TO "r0797739";
grant all on schema "R1TX32_team02" TO "r???????";
grant all on schema "R1TX32_team02" TO "r???????";
```
### Het instellen van het correcte search path
```
SET search_path TO R1TX32_team02;
```
 > TIP!
Als je een CREATE TABLE statement toevoegt in je CREATE script (na testen van dit statement), voeg dan ineens ook de DROP TABLE statement vooraan toe in je DROP script. 
Zo ben je zeker dat de volgorde correct is. 
Als je dan iets wil aanpassen in een tabel, pas dan ineens aan in het CREATE script en laat dan eerst het DROP script runnen en het volledige CREATE script. Zo ben je ook zeker dat er zich geen fouten voordoen (of kan je ze onmiddellijk oplossen)

### Aanmaken van de tabbelen
```
CREATE TABLE IF NOT EXISTS R1TX32_team02.klanten (
  id INT NOT NULL,
  voornaam text NOT NULL,
  achternaam text NOT NULL,
  straatnaam text NOT NULL,
  huisnummer text NOT NULL,
  gemeente text NOT NULL,
  postcode text NOT NULL,
  PRIMARY KEY (id)
  );

CREATE TABLE IF NOT EXISTS R1TX32_team02.bungalowpark (
  id INT NOT NULL,
  straat text NULL,
  huisnummer text NULL,
  postcode text NULL,
  gemeente text NULL,
  PRIMARY KEY (id)
  );

CREATE TABLE IF NOT EXISTS R1TX32_team02.periode (
  id INT NOT NULL,
  duur text NULL,
  datum date NULL,
  seizoen text NULL,
  PRIMARY KEY (id)
  );

CREATE TABLE IF NOT EXISTS R1TX32_team02.bungalowtype (
  id INT NOT NULL,
  klasse text NULL,
  capaciteit INT NULL,
  PRIMARY KEY (id)
  );

CREATE TABLE IF NOT EXISTS R1TX32_team02.zone (
  id INT NOT NULL,
  uitzicht text NULL,
  nabijheid text NULL,
  PRIMARY KEY (id)
  );

CREATE TABLE IF NOT EXISTS R1TX32_team02.bungalow (
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
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTIxNzM4ODU0MiwyMDgxODUzNjM1LDE4Nz
czOTE5MTldfQ==
-->