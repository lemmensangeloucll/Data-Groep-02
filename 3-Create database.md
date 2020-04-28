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


```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI1MjAzNzY1MywyMDgxODUzNjM1LDE4Nz
czOTE5MTldfQ==
-->