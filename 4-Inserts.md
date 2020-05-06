## Inserts into

### Recourse
> https://www.generatedata.com/


> https://mockaroo.com

### Aantallen voor de database structuur

> Aantal reservaties -> 100 000
> Contacttypes -> 3 (telefonisch, email, on-site)
> Bungalowparken -> 8
> Periodes -> 4
> Bungalowtypes -> 4
> Klanten -> 100 000
> Bungalows -> 15

### Straatnamen
```
Mussenstraat|Ravenstraat|Bondgenotenlaan|Martelarenplein|Parijsstraat|Urselweg|Kemmelbergstraat
```
### Gemeentes
```
Leuven|Knokke-Heist|Kessel-lo|Maldegem|Wilsele|Tienen|Tielt-Winge|Diest|Begijnendijk|Geetbets
```

## Inserts
### Klanten
```
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (1,'Lavinia','Ramos','Urselweg',35,'Maldegem','5452'),(2,'Clarke','Dean','Urselweg',152,'Diest','7083'),(3,'Linda','Gates','Parijsstraat',249,'Kessel-lo','4997'),(4,'Hadassah','Shepherd','Urselweg',228,'Tienen','6388'),(5,'Kibo','Foley','Bondgenotenlaan',189,'Diest','2134'),(6,'Alisa','Wilkinson','Kemmelbergstraat',215,'Leuven','6454'),(7,'Jonas','Burgess','Ravenstraat',144,'Knokke-Heist','5858'),(8,'Chelsea','Morrison','Martelarenplein',83,'Leuven','1576'),(9,'Tatyana','Ortiz','Kemmelbergstraat',157,'Tielt-Winge','8480'),(10,'Gage','Bass','Kemmelbergstraat',22,'Tielt-Winge','6381');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (11,'Lester','Nolan','Martelarenplein',163,'Tielt-Winge','7985'),(12,'Cynthia','Sloan','Urselweg',12,'Knokke-Heist','2548'),(13,'Iliana','Ware','Urselweg',4,'Knokke-Heist','1271'),(14,'Christen','Salas','Kemmelbergstraat',216,'Maldegem','5579'),(15,'Nyssa','Wheeler','Urselweg',245,'Kessel-lo','5112'),(16,'Maggy','Dunn','Parijsstraat',176,'Begijnendijk','9013'),(17,'Cairo','Gates','Martelarenplein',204,'Tielt-Winge','4864'),(18,'Summer','Garrison','Ravenstraat',193,'Knokke-Heist','1015'),(19,'Brennan','Rivera','Martelarenplein',197,'Diest','5094'),(20,'Hilda','Pratt','Martelarenplein',127,'Kessel-lo','5419');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (21,'Nelle','Wright','Mussenstraat',116,'Knokke-Heist','5988'),(22,'Alisa','Stevens','Bondgenotenlaan',63,'Tielt-Winge','4685'),(23,'Gay','Snider','Parijsstraat',163,'Geetbets','9787'),(24,'Ivy','English','Bondgenotenlaan',141,'Leuven','5174'),(25,'John','Bernard','Ravenstraat',141,'Knokke-Heist','4725'),(26,'Anjolie','Bond','Mussenstraat',57,'Diest','2621'),(27,'Adrian','Hester','Ravenstraat',172,'Wilsele','4603'),(28,'Reed','Salinas','Kemmelbergstraat',163,'Kessel-lo','1030'),(29,'Kessie','Fernandez','Mussenstraat',69,'Tienen','4911'),(30,'Myles','Harvey','Kemmelbergstraat',148,'Tielt-Winge','3185');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (31,'Ralph','Bernard','Urselweg',65,'Knokke-Heist','5275'),(32,'Yeo','Odonnell','Bondgenotenlaan',46,'Knokke-Heist','6765'),(33,'David','Sandoval','Mussenstraat',116,'Begijnendijk','3853'),(34,'Fiona','Alexander','Parijsstraat',166,'Leuven','8395'),(35,'Alana','Dunlap','Kemmelbergstraat',138,'Tielt-Winge','9334'),(36,'Kenneth','Long','Kemmelbergstraat',129,'Tielt-Winge','8553'),(37,'Carolyn','Merritt','Ravenstraat',128,'Wilsele','5317'),(38,'Whitney','Reilly','Bondgenotenlaan',10,'Geetbets','8312'),(39,'Rina','Benson','Urselweg',124,'Maldegem','3993'),(40,'Breanna','Guy','Bondgenotenlaan',54,'Tienen','7390');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (41,'Herman','Holt','Bondgenotenlaan',226,'Wilsele','4638'),(42,'Winifred','Steele','Parijsstraat',25,'Leuven','2917'),(43,'Rhona','Washington','Bondgenotenlaan',74,'Knokke-Heist','7713'),(44,'Guy','Mayo','Parijsstraat',9,'Tielt-Winge','5644'),(45,'Dai','Abbott','Kemmelbergstraat',60,'Knokke-Heist','4193'),(46,'Amela','Lloyd','Urselweg',185,'Tielt-Winge','7571'),(47,'Demetrius','Vega','Martelarenplein',84,'Kessel-lo','5692'),(48,'Jonah','Patel','Urselweg',74,'Kessel-lo','5606'),(49,'Cedric','Henderson','Ravenstraat',113,'Diest','9275'),(50,'Wylie','Jordan','Parijsstraat',55,'Geetbets','5242');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (51,'Germaine','Arnold','Urselweg',196,'Leuven','6229'),(52,'Hermione','Gates','Urselweg',242,'Begijnendijk','8648'),(53,'Joel','Mullins','Ravenstraat',187,'Leuven','5745'),(54,'Laurel','Rush','Martelarenplein',17,'Diest','9853'),(55,'Brenna','Parsons','Mussenstraat',56,'Tienen','9618'),(56,'Xenos','Forbes','Martelarenplein',197,'Maldegem','8689'),(57,'Shea','Larson','Mussenstraat',215,'Diest','3110'),(58,'Shana','Bates','Martelarenplein',6,'Tienen','9633'),(59,'Jena','Boone','Urselweg',22,'Knokke-Heist','2142'),(60,'Gloria','Hunter','Ravenstraat',24,'Knokke-Heist','6703');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (61,'Samson','Puckett','Ravenstraat',2,'Geetbets','7120'),(62,'Callum','Russo','Ravenstraat',176,'Wilsele','6092'),(63,'Harrison','Carter','Bondgenotenlaan',119,'Knokke-Heist','3822'),(64,'Alisa','Porter','Kemmelbergstraat',16,'Knokke-Heist','2542'),(65,'Kimberley','Mccarthy','Bondgenotenlaan',63,'Tielt-Winge','5543'),(66,'Nadine','Flores','Ravenstraat',57,'Geetbets','8787'),(67,'Maile','Hamilton','Parijsstraat',182,'Wilsele','6588'),(68,'Geraldine','Barker','Ravenstraat',23,'Tielt-Winge','1481'),(69,'Teagan','Freeman','Mussenstraat',168,'Tienen','8834'),(70,'Jerome','Patel','Mussenstraat',124,'Wilsele','4357');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (71,'Keely','William','Martelarenplein',113,'Diest','3473'),(72,'Lee','Logan','Bondgenotenlaan',119,'Leuven','3293'),(73,'Olympia','Walton','Martelarenplein',27,'Begijnendijk','8020'),(74,'Quamar','Gates','Parijsstraat',43,'Begijnendijk','4643'),(75,'Hermione','Mccarthy','Parijsstraat',90,'Maldegem','3288'),(76,'Kim','Maddox','Martelarenplein',188,'Begijnendijk','8311'),(77,'Peter','Parrish','Kemmelbergstraat',196,'Kessel-lo','8405'),(78,'Willow','Mack','Ravenstraat',149,'Diest','2137'),(79,'Owen','Bailey','Martelarenplein',118,'Tielt-Winge','7653'),(80,'Leila','Powers','Bondgenotenlaan',239,'Tielt-Winge','1092');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (81,'Ramona','Moses','Ravenstraat',250,'Tienen','6188'),(82,'Athena','Cole','Urselweg',25,'Knokke-Heist','6585'),(83,'Conan','Rogers','Parijsstraat',81,'Tienen','6700'),(84,'Devin','Roth','Parijsstraat',150,'Geetbets','9730'),(85,'Rhea','Mcclure','Martelarenplein',4,'Leuven','7543'),(86,'Noble','Green','Kemmelbergstraat',6,'Begijnendijk','7409'),(87,'Flavia','Finley','Bondgenotenlaan',159,'Leuven','3595'),(88,'Deacon','Hatfield','Ravenstraat',98,'Knokke-Heist','8675'),(89,'Forrest','Lindsey','Mussenstraat',173,'Tielt-Winge','5217'),(90,'Gregory','Jefferson','Bondgenotenlaan',229,'Maldegem','1989');
INSERT INTO "klanten" (id,voornaam,achternaam,straatnaam,huisnummer,gemeente,postcode) VALUES (91,'Madaline','Barlow','Urselweg',22,'Geetbets','7724'),(92,'Russell','Maxwell','Bondgenotenlaan',151,'Tienen','4452'),(93,'Slade','Rodriguez','Parijsstraat',230,'Knokke-Heist','8316'),(94,'Halee','Valdez','Urselweg',215,'Begijnendijk','7012'),(95,'Xerxes','Delgado','Bondgenotenlaan',198,'Leuven','1173'),(96,'Timothy','Summers','Mussenstraat',158,'Tienen','2843'),(97,'Ryan','Joyner','Martelarenplein',182,'Begijnendijk','2326'),(98,'Jacob','Cook','Ravenstraat',249,'Knokke-Heist','3745'),(99,'Thomas','Fuller','Parijsstraat',122,'Maldegem','7552'),(100,'Summer','Mathis','Mussenstraat',148,'Tienen','1694');
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ5NTA3OTE0MywtNTQ0NTgwMDgzLDE4NT
QzNTI0MjksNjYzNTMyODksLTk1NTI0OTEwN119
-->