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

> huisnummer -> 500

>postcode -> 1000 -> 9999

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
### Facturen
```
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (1, '2020/541655', 'congue diam id ornare imperdiet sapien urna pretium nisl', 599.02, 125.79, null, 724.81, 1);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (2, '2020/895632', 'augue vestibulum rutrum rutrum', 1645.34, 345.52, 102.09, 1990.86, 2);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (3, '2020/657428', 'magna', 254.8, 53.51, null, 308.31, 3);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (4, '2020/236461', 'ut nulla sed accumsan felis', 3197.87, 671.55, 69.14, 3869.42, 4);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (5, '2020/273431', 'vivamus in felis eu sapien cursus vestibulum', 2814.13, 590.97, 20.86, 3405.1, 5);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (6, '2020/274396', 'nisl ut', 2101.63, 441.34, 77.71, 2542.97, 6);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (7, '2020/823422', 'integer ac leo pellentesque ultrices mattis odio donec vitae', 1705.12, 358.08, null, 2063.2, 7);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (8, '2020/728246', 'tristique', 1144.43, 240.33, null, 1384.76, 8);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (9, '2020/445577', 'justo etiam pretium iaculis justo in hac habitasse platea dictumst', 2368.26, 497.33, 92.39, 2865.59, 9);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (10, '2020/689400', 'quam fringilla rhoncus mauris enim', 871.59, 183.03, null, 1054.62, 10);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (11, '2020/096536', 'porttitor lorem', 279.56, 58.71, 81.19, 338.27, 11);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (12, '2020/151184', 'velit donec diam neque vestibulum eget vulputate ut ultrices vel', 771.01, 161.91, null, 932.92, 12);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (13, '2020/037011', 'dolor vel est donec odio justo sollicitudin ut suscipit', 3104.8, 652.01, 136.06, 3756.81, 13);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (14, '2020/311917', 'suspendisse potenti in eleifend quam a odio in hac habitasse', 3309.56, 695.01, null, 4004.57, 14);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (15, '2020/401015', 'mauris non ligula pellentesque ultrices phasellus id', 695.37, 146.03, null, 841.4, 15);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (16, '2020/536366', 'sapien urna pretium nisl ut volutpat sapien arcu', 1837.24, 385.82, null, 2223.06, 16);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (17, '2020/174332', 'justo nec condimentum neque sapien placerat ante nulla justo aliquam', 497.81, 104.54, 111.4, 602.35, 17);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (18, '2020/676694', 'habitasse platea dictumst maecenas ut', 2726.24, 572.51, 66.48, 3298.75, 18);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (19, '2020/816989', 'donec', 840.67, 176.54, null, 1017.21, 19);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (20, '2020/745164', 'ipsum dolor sit amet consectetuer adipiscing elit', 1229.92, 258.28, null, 1488.2, 20);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (21, '2020/463127', 'nibh quisque', 1348.9, 283.27, 47.82, 1632.17, 21);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (22, '2020/153376', 'ultrices erat tortor sollicitudin mi sit amet lobortis sapien', 527.1, 110.69, null, 637.79, 22);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (23, '2020/657608', 'id ornare imperdiet sapien urna pretium nisl ut volutpat', 3286.15, 690.09, null, 3976.24, 23);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (24, '2020/694657', 'urna pretium nisl', 1664.63, 349.57, null, 2014.2, 24);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (25, '2020/374241', 'nam nulla integer pede justo lacinia eget tincidunt eget tempus', 3323.12, 697.86, null, 4020.98, 25);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (26, '2020/810924', 'ullamcorper augue a suscipit nulla elit ac nulla', 2117.73, 444.72, 59.95, 2562.45, 26);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (27, '2020/716594', 'augue a', 2983.33, 626.5, 44.66, 3609.83, 27);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (28, '2020/627204', 'sapien cum sociis natoque penatibus et magnis dis parturient', 2833.69, 595.07, null, 3428.76, 28);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (29, '2020/975656', 'a suscipit nulla elit ac nulla sed', 2505.01, 526.05, 144.7, 3031.06, 29);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (30, '2020/731804', 'sit amet', 1793.84, 376.71, null, 2170.55, 30);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (31, '2020/150572', 'nec nisi vulputate nonummy maecenas tincidunt', 609.84, 128.07, 74.18, 737.91, 31);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (32, '2020/068233', 'vestibulum sit amet cursus id turpis integer aliquet massa id', 3434.39, 721.22, 19.29, 4155.61, 32);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (33, '2020/392408', 'faucibus orci luctus et ultrices posuere cubilia curae mauris', 1932.2, 405.76, null, 2337.96, 33);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (34, '2020/213162', 'ornare imperdiet sapien urna pretium nisl', 1529.11, 321.11, 58.98, 1850.22, 34);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (35, '2020/543325', 'ipsum integer a nibh in quis justo', 433.71, 91.08, null, 524.79, 35);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (36, '2020/132507', 'sit amet nulla quisque arcu libero rutrum', 2924.56, 614.16, 88.0, 3538.72, 36);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (37, '2020/067321', 'tincidunt ante vel ipsum', 1222.15, 256.65, null, 1478.8, 37);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (38, '2020/728891', 'eget', 1519.48, 319.09, null, 1838.57, 38);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (39, '2020/475560', 'nunc vestibulum ante ipsum primis in faucibus orci luctus', 1655.21, 347.59, null, 2002.8, 39);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (40, '2020/646725', 'primis in faucibus orci luctus et ultrices posuere', 2347.85, 493.05, null, 2840.9, 40);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (41, '2020/530860', 'dictumst etiam faucibus cursus', 1295.81, 272.12, 36.23, 1567.93, 41);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (42, '2020/423489', 'pede justo lacinia eget tincidunt eget', 1828.4, 383.96, null, 2212.36, 42);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (43, '2020/370318', 'sit amet turpis elementum ligula vehicula consequat morbi', 3340.73, 701.55, null, 4042.28, 43);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (44, '2020/727546', 'felis donec semper sapien a libero', 1233.73, 259.08, null, 1492.81, 44);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (45, '2020/812908', 'hac habitasse platea dictumst', 782.79, 164.39, null, 947.18, 45);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (46, '2020/150558', 'ipsum', 3215.61, 675.28, 60.84, 3890.89, 46);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (47, '2020/261985', 'ante ipsum primis in faucibus orci luctus', 2311.96, 485.51, 111.39, 2797.47, 47);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (48, '2020/340391', 'ipsum dolor sit', 3188.29, 669.54, null, 3857.83, 48);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (49, '2020/600672', 'donec dapibus duis at velit eu est congue elementum in', 3061.11, 642.83, null, 3703.94, 49);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (50, '2020/277700', 'et magnis dis parturient montes nascetur ridiculus', 3387.82, 711.44, null, 4099.26, 50);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (51, '2020/172384', 'aliquam', 2117.94, 444.77, 99.79, 2562.71, 51);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (52, '2020/501506', 'metus aenean fermentum donec ut mauris eget massa', 2561.51, 537.92, 86.83, 3099.43, 52);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (53, '2020/786673', 'faucibus orci luctus et ultrices posuere cubilia curae nulla', 2790.13, 585.93, null, 3376.06, 53);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (54, '2020/344280', 'morbi quis tortor', 2282.86, 479.4, null, 2762.26, 54);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (55, '2020/164716', 'accumsan', 2037.49, 427.87, 87.83, 2465.36, 55);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (56, '2020/359271', 'molestie lorem quisque ut', 606.68, 127.4, 56.44, 734.08, 56);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (57, '2020/533809', 'ac', 692.6, 145.45, null, 838.05, 57);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (58, '2020/499651', 'vestibulum ante ipsum primis in', 2647.79, 556.04, null, 3203.83, 58);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (59, '2020/106071', 'enim in tempor turpis nec euismod scelerisque quam', 801.15, 168.24, 53.26, 969.39, 59);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (60, '2020/702297', 'eget nunc donec', 2651.83, 556.88, null, 3208.71, 60);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (61, '2020/128909', 'orci nullam molestie nibh in lectus pellentesque at nulla suspendisse', 2253.48, 473.23, null, 2726.71, 61);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (62, '2020/059248', 'faucibus orci luctus et ultrices', 2373.98, 498.54, null, 2872.52, 62);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (63, '2020/188551', 'eu sapien cursus vestibulum', 1065.72, 223.8, null, 1289.52, 63);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (64, '2020/960051', 'turpis sed ante vivamus', 1313.11, 275.75, 11.09, 1588.86, 64);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (65, '2020/921413', 'lobortis convallis tortor risus', 2659.93, 558.59, 50.22, 3218.52, 65);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (66, '2020/158694', 'ut', 273.53, 57.44, null, 330.97, 66);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (67, '2020/745423', 'rhoncus sed vestibulum sit amet cursus id', 2492.48, 523.42, 145.49, 3015.9, 67);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (68, '2020/322470', 'nulla pede ullamcorper augue a suscipit nulla', 3308.11, 694.7, null, 4002.81, 68);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (69, '2020/782464', 'vel pede morbi', 1142.54, 239.93, null, 1382.47, 69);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (70, '2020/577401', 'ultrices posuere cubilia curae duis faucibus accumsan odio', 2259.16, 474.42, null, 2733.58, 70);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (71, '2020/155568', 'fusce congue diam', 557.92, 117.16, null, 675.08, 71);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (72, '2020/845274', 'hac habitasse platea dictumst maecenas ut massa quis augue', 3349.7, 703.44, null, 4053.14, 72);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (73, '2020/366581', 'massa id nisl venenatis lacinia aenean sit amet justo morbi', 540.64, 113.53, null, 654.17, 73);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (74, '2020/680084', 'leo odio condimentum id luctus nec molestie sed justo', 1739.28, 365.25, null, 2104.53, 74);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (75, '2020/723261', 'volutpat erat', 366.7, 77.01, null, 443.71, 75);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (76, '2020/033732', 'metus vitae ipsum aliquam non mauris morbi non lectus', 1086.62, 228.19, 59.58, 1314.81, 76);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (77, '2020/908454', 'id ornare imperdiet sapien urna pretium nisl ut', 2119.61, 445.12, null, 2564.73, 77);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (78, '2020/177122', 'sapien dignissim vestibulum vestibulum ante', 2826.34, 593.53, null, 3419.87, 78);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (79, '2020/466123', 'curabitur convallis duis', 1406.0, 295.26, null, 1701.26, 79);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (80, '2020/017359', 'lectus suspendisse potenti in eleifend quam a', 3420.95, 718.4, 107.37, 4139.35, 80);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (81, '2020/081236', 'tempus semper est quam pharetra magna ac consequat metus', 2096.34, 440.23, 10.15, 2536.57, 81);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (82, '2020/737563', 'euismod scelerisque quam', 1100.67, 231.14, null, 1331.81, 82);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (83, '2020/388056', 'commodo vulputate justo', 3382.09, 710.24, null, 4092.33, 83);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (84, '2020/039863', 'aliquam augue', 607.25, 127.52, null, 734.77, 84);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (85, '2020/480059', 'eu nibh quisque id justo sit amet sapien dignissim', 1917.97, 402.77, null, 2320.74, 85);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (86, '2020/478815', 'blandit lacinia erat vestibulum sed magna at', 2438.52, 512.09, null, 2950.61, 86);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (87, '2020/332352', 'erat', 2487.6, 522.4, null, 3010.0, 87);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (88, '2020/842107', 'eu tincidunt in leo maecenas pulvinar', 1879.28, 394.65, 19.3, 2273.93, 88);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (89, '2020/045222', 'molestie nibh', 1674.38, 351.62, null, 2026.0, 89);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (90, '2020/200188', 'in est risus auctor sed tristique in', 1165.45, 244.74, null, 1410.19, 90);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (91, '2020/069401', 'eu felis fusce', 626.05, 131.47, null, 757.52, 91);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (92, '2020/194613', 'diam in magna bibendum imperdiet nullam orci', 1867.55, 392.19, 132.11, 2259.74, 92);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (93, '2020/814896', 'auctor sed tristique in tempus sit amet sem', 3179.79, 667.76, 69.03, 3847.55, 93);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (94, '2020/261964', 'ullamcorper augue a suscipit', 3410.96, 716.3, null, 4127.26, 94);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (95, '2020/846856', 'tortor sollicitudin mi sit amet lobortis sapien', 1929.9, 405.28, null, 2335.18, 95);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (96, '2020/617589', 'suscipit a feugiat et eros vestibulum ac est lacinia nisi', 990.63, 208.03, 147.76, 1198.66, 96);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (97, '2020/959902', 'consequat nulla nisl nunc nisl duis bibendum felis sed', 1240.17, 260.44, null, 1500.61, 97);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (98, '2020/737009', 'venenatis', 902.25, 189.47, null, 1091.72, 98);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (99, '2020/163223', 'ipsum aliquam non', 2200.91, 462.19, null, 2663.1, 99);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (100, '2020/443457', 'curae donec pharetra magna vestibulum aliquet ultrices', 3312.4, 695.6, 22.39, 4008.0, 100);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (101, '2020/230535', 'integer pede justo lacinia eget tincidunt', 1467.03, 308.08, null, 1775.11, 101);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (102, '2020/502755', 'interdum venenatis', 963.32, 202.3, 99.68, 1165.62, 102);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (103, '2020/852428', 'mi integer', 1394.07, 292.75, null, 1686.82, 103);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (104, '2020/583369', 'maecenas tristique est et tempus', 1102.57, 231.54, null, 1334.11, 104);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (105, '2020/979990', 'sit amet justo morbi ut odio cras mi', 1779.57, 373.71, null, 2153.28, 105);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (106, '2020/937147', 'parturient montes nascetur ridiculus mus vivamus vestibulum', 1606.86, 337.44, 83.52, 1944.3, 106);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (107, '2020/308579', 'vestibulum quam sapien varius ut blandit', 3383.91, 710.62, 143.41, 4094.53, 107);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (108, '2020/380652', 'sed', 3382.9, 710.41, 36.24, 4093.31, 108);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (109, '2020/641591', 'non pretium quis lectus suspendisse potenti in', 1147.75, 241.03, 132.72, 1388.78, 109);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (110, '2020/253649', 'vivamus in felis eu sapien cursus vestibulum proin eu mi', 3220.16, 676.23, null, 3896.39, 110);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (111, '2020/282885', 'tortor duis mattis egestas metus aenean', 1944.46, 408.34, null, 2352.8, 111);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (112, '2020/260748', 'aliquam erat volutpat in congue', 3433.73, 721.08, null, 4154.81, 112);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (113, '2020/369692', 'risus', 844.12, 177.27, 10.42, 1021.39, 113);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (114, '2020/339780', 'mauris vulputate elementum', 1212.66, 254.66, 102.76, 1467.32, 114);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (115, '2020/158379', 'quam sapien varius ut blandit non interdum in ante vestibulum', 2624.39, 551.12, null, 3175.51, 115);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (116, '2020/423729', 'consequat nulla', 2525.41, 530.34, 86.23, 3055.75, 116);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (117, '2020/418326', 'suspendisse potenti', 2885.65, 605.99, null, 3491.64, 117);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (118, '2020/815231', 'pulvinar nulla pede ullamcorper augue a suscipit nulla elit ac', 565.14, 118.68, 18.4, 683.82, 118);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (119, '2020/250563', 'habitasse platea dictumst aliquam augue', 504.39, 105.92, null, 610.31, 119);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (120, '2020/307564', 'massa id lobortis convallis tortor', 713.33, 149.8, 94.93, 863.13, 120);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (121, '2020/205758', 'nulla sed vel', 2330.25, 489.35, 71.37, 2819.6, 121);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (122, '2020/917725', 'etiam pretium iaculis justo in hac habitasse platea', 2833.9, 595.12, 13.87, 3429.02, 122);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (123, '2020/774970', 'aenean lectus', 2527.71, 530.82, null, 3058.53, 123);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (124, '2020/934992', 'risus dapibus augue vel accumsan tellus', 1646.61, 345.79, null, 1992.4, 124);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (125, '2020/635895', 'libero nam dui proin leo', 2701.55, 567.33, null, 3268.88, 125);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (126, '2020/880563', 'fermentum justo nec condimentum neque sapien placerat ante nulla', 1334.02, 280.14, null, 1614.16, 126);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (127, '2020/425219', 'adipiscing molestie hendrerit at', 1754.15, 368.37, null, 2122.52, 127);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (128, '2020/341507', 'habitasse platea dictumst etiam faucibus cursus urna ut tellus', 442.39, 92.9, null, 535.29, 128);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (129, '2020/313430', 'magna at nunc commodo placerat praesent blandit nam nulla integer', 1030.87, 216.48, 129.39, 1247.35, 129);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (130, '2020/059346', 'ante ipsum primis in faucibus orci luctus et ultrices', 2869.56, 602.61, null, 3472.17, 130);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (131, '2020/951730', 'in quam fringilla rhoncus mauris', 1263.13, 265.26, null, 1528.39, 131);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (132, '2020/834112', 'mauris viverra diam vitae quam suspendisse potenti nullam porttitor lacus', 1634.32, 343.21, null, 1977.53, 132);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (133, '2020/391548', 'felis', 3484.04, 731.65, 18.31, 4215.69, 133);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (134, '2020/002409', 'arcu', 1835.99, 385.56, 105.49, 2221.55, 134);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (135, '2020/055109', 'vestibulum ante ipsum primis in faucibus orci luctus et ultrices', 1951.74, 409.87, 4.2, 2361.61, 135);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (136, '2020/343868', 'at vulputate vitae nisl aenean lectus pellentesque eget nunc donec', 3350.42, 703.59, 18.53, 4054.01, 136);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (137, '2020/313106', 'morbi non quam nec dui luctus rutrum nulla', 848.65, 178.22, 103.09, 1026.87, 137);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (138, '2020/900968', 'erat eros viverra eget congue eget semper rutrum', 1636.45, 343.65, 38.77, 1980.1, 138);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (139, '2020/936942', 'dapibus dolor vel est donec odio justo sollicitudin ut suscipit', 1850.52, 388.61, null, 2239.13, 139);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (140, '2020/516665', 'orci eget orci', 1645.03, 345.46, null, 1990.49, 140);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (141, '2020/235777', 'eros vestibulum ac est', 481.59, 101.13, 60.82, 582.72, 141);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (142, '2020/918113', 'sed sagittis nam congue risus semper porta volutpat quam', 1212.43, 254.61, null, 1467.04, 142);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (143, '2020/647407', 'odio justo sollicitudin ut suscipit a feugiat et eros vestibulum', 411.27, 86.37, 65.57, 497.64, 143);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (144, '2020/195880', 'ridiculus mus vivamus vestibulum sagittis', 1464.11, 307.46, 37.35, 1771.57, 144);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (145, '2020/905700', 'curabitur at', 1205.77, 253.21, null, 1458.98, 145);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (146, '2020/404497', 'mauris non ligula pellentesque ultrices phasellus id sapien in', 2597.27, 545.43, 135.24, 3142.7, 146);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (147, '2020/808795', 'sollicitudin ut suscipit a feugiat et', 1938.96, 407.18, null, 2346.14, 147);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (148, '2020/737805', 'eu interdum eu', 1647.9, 346.06, null, 1993.96, 148);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (149, '2020/413546', 'nulla suscipit ligula in lacus curabitur', 2304.47, 483.94, null, 2788.41, 149);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (150, '2020/750572', 'est lacinia nisi venenatis tristique fusce congue', 2062.92, 433.21, 9.84, 2496.13, 150);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (151, '2020/244510', 'ac nibh fusce lacus', 2839.21, 596.23, 42.52, 3435.44, 151);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (152, '2020/762795', 'nisl ut volutpat sapien arcu sed augue aliquam erat volutpat', 518.24, 108.83, null, 627.07, 152);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (153, '2020/978642', 'etiam pretium iaculis', 1866.42, 391.95, null, 2258.37, 153);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (154, '2020/907341', 'leo', 3324.34, 698.11, 102.51, 4022.45, 154);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (155, '2020/793927', 'suscipit nulla elit ac', 2332.41, 489.81, null, 2822.22, 155);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (156, '2020/347225', 'quam nec dui luctus rutrum nulla tellus in sagittis', 2066.19, 433.9, 104.32, 2500.09, 156);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (157, '2020/993443', 'est et tempus semper est quam pharetra magna', 3054.35, 641.41, 75.35, 3695.76, 157);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (158, '2020/829624', 'nunc rhoncus dui vel sem sed', 1511.23, 317.36, null, 1828.59, 158);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (159, '2020/799012', 'gravida nisi at nibh in hac habitasse platea', 2539.0, 533.19, 30.74, 3072.19, 159);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (160, '2020/714154', 'duis ac nibh fusce lacus purus aliquet at feugiat non', 3303.01, 693.63, 1.38, 3996.64, 160);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (161, '2020/686946', 'posuere nonummy integer non', 2490.23, 522.95, null, 3013.18, 161);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (162, '2020/701171', 'platea dictumst', 497.29, 104.43, 136.51, 601.72, 162);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (163, '2020/053291', 'rutrum', 475.78, 99.91, 127.71, 575.69, 163);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (164, '2020/541225', 'aliquet ultrices erat tortor', 2090.77, 439.06, null, 2529.83, 164);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (165, '2020/606169', 'odio curabitur convallis', 2861.3, 600.87, null, 3462.17, 165);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (166, '2020/065643', 'tortor sollicitudin mi', 615.98, 129.36, null, 745.34, 166);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (167, '2020/784057', 'justo lacinia eget tincidunt eget tempus vel pede', 2896.43, 608.25, null, 3504.68, 167);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (168, '2020/641204', 'sit amet', 2564.1, 538.46, 146.69, 3102.56, 168);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (169, '2020/483234', 'dolor', 3089.93, 648.89, 79.09, 3738.82, 169);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (170, '2020/975752', 'varius nulla facilisi cras non velit nec nisi', 3027.34, 635.74, 118.56, 3663.08, 170);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (171, '2020/760942', 'vestibulum eget vulputate', 2180.95, 458.0, 51.68, 2638.95, 171);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (172, '2020/499995', 'vivamus vel nulla eget eros elementum pellentesque', 461.53, 96.92, null, 558.45, 172);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (173, '2020/498131', 'ultrices phasellus id sapien in sapien iaculis congue vivamus metus', 2243.45, 471.12, null, 2714.57, 173);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (174, '2020/159056', 'etiam pretium iaculis justo', 3122.72, 655.77, null, 3778.49, 174);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (175, '2020/094700', 'justo etiam pretium iaculis justo in hac habitasse platea dictumst', 1629.28, 342.15, null, 1971.43, 175);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (176, '2020/026118', 'luctus et ultrices posuere cubilia', 3048.59, 640.2, null, 3688.79, 176);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (177, '2020/021280', 'arcu sed augue aliquam erat volutpat in congue', 2690.14, 564.93, 7.03, 3255.07, 177);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (178, '2020/478777', 'eleifend donec', 2509.72, 527.04, 149.87, 3036.76, 178);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (179, '2020/690743', 'non mauris morbi', 3019.44, 634.08, 40.28, 3653.52, 179);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (180, '2020/396980', 'magnis dis parturient montes nascetur ridiculus mus etiam', 1482.72, 311.37, null, 1794.09, 180);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (181, '2020/786478', 'est phasellus sit amet erat nulla', 3459.31, 726.46, null, 4185.77, 181);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (182, '2020/322202', 'in est risus auctor sed tristique in tempus', 3343.95, 702.23, null, 4046.18, 182);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (183, '2020/830789', 'integer tincidunt ante vel ipsum praesent blandit lacinia erat', 2826.38, 593.54, null, 3419.92, 183);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (184, '2020/850039', 'quisque id', 298.73, 62.73, 26.43, 361.46, 184);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (185, '2020/305167', 'in purus eu magna vulputate', 1502.82, 315.59, null, 1818.41, 185);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (186, '2020/828869', 'at turpis donec posuere metus vitae', 1686.74, 354.22, null, 2040.96, 186);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (187, '2020/882610', 'vulputate vitae nisl aenean lectus pellentesque eget', 1579.05, 331.6, 1.65, 1910.65, 187);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (188, '2020/590892', 'sit amet sem fusce', 1661.62, 348.94, 107.59, 2010.56, 188);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (189, '2020/876969', 'molestie nibh in lectus', 3499.97, 734.99, 93.12, 4234.96, 189);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (190, '2020/978955', 'turpis sed ante vivamus', 294.87, 61.92, null, 356.79, 190);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (191, '2020/585681', 'pede posuere nonummy integer', 2147.39, 450.95, null, 2598.34, 191);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (192, '2020/527212', 'metus sapien ut nunc vestibulum ante ipsum', 2727.49, 572.77, null, 3300.26, 192);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (193, '2020/469015', 'libero quis orci', 3339.16, 701.22, 132.12, 4040.38, 193);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (194, '2020/730537', 'est', 1613.87, 338.91, null, 1952.78, 194);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (195, '2020/936585', 'blandit lacinia erat vestibulum sed magna at', 322.17, 67.66, 107.49, 389.83, 195);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (196, '2020/915596', 'eu felis fusce posuere felis sed lacus morbi sem mauris', 2673.17, 561.37, 92.01, 3234.54, 196);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (197, '2020/773058', 'consequat ut nulla', 541.38, 113.69, 123.55, 655.07, 197);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (198, '2020/982090', 'consectetuer eget rutrum at lorem integer tincidunt ante vel ipsum', 1809.9, 380.08, 136.4, 2189.98, 198);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (199, '2020/432453', 'vestibulum velit id pretium iaculis diam erat', 1171.3, 245.97, 68.87, 1417.27, 199);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (200, '2020/363043', 'dui', 1593.08, 334.55, 94.56, 1927.63, 200);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (201, '2020/200592', 'eget eros elementum pellentesque quisque porta', 1731.24, 363.56, 94.41, 2094.8, 201);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (202, '2020/365721', 'vestibulum aliquet ultrices erat tortor', 2995.2, 628.99, 59.83, 3624.19, 202);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (203, '2020/143373', 'phasellus', 320.58, 67.32, 86.29, 387.9, 203);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (204, '2020/257399', 'velit eu est congue elementum in', 3184.84, 668.82, null, 3853.66, 204);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (205, '2020/502422', 'lectus in est risus auctor', 2782.55, 584.34, 120.24, 3366.89, 205);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (206, '2020/253639', 'duis mattis egestas metus aenean fermentum donec ut mauris eget', 250.18, 52.54, 63.29, 302.72, 206);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (207, '2020/028375', 'lacinia aenean sit amet justo morbi ut', 2992.3, 628.38, 121.79, 3620.68, 207);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (208, '2020/878189', 'faucibus orci luctus et ultrices posuere cubilia curae mauris viverra', 787.19, 165.31, null, 952.5, 208);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (209, '2020/029413', 'tempus vel pede morbi', 2564.73, 538.59, null, 3103.32, 209);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (210, '2020/817459', 'ac est lacinia nisi venenatis tristique', 2186.94, 459.26, 118.66, 2646.2, 210);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (211, '2020/984534', 'cum sociis natoque penatibus et magnis', 1124.99, 236.25, 122.72, 1361.24, 211);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (212, '2020/580514', 'et ultrices posuere cubilia curae mauris viverra', 3138.55, 659.1, null, 3797.65, 212);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (213, '2020/323468', 'nulla suscipit ligula in lacus', 1755.02, 368.55, null, 2123.57, 213);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (214, '2020/592262', 'tempus sit amet sem fusce', 2807.09, 589.49, 45.94, 3396.58, 214);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (215, '2020/292493', 'ridiculus mus etiam vel augue vestibulum', 1979.3, 415.65, null, 2394.95, 215);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (216, '2020/629454', 'vestibulum quam sapien', 1647.51, 345.98, null, 1993.49, 216);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (217, '2020/599839', 'tortor id nulla', 1399.28, 293.85, null, 1693.13, 217);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (218, '2020/056504', 'sed tristique in tempus sit amet', 1854.2, 389.38, null, 2243.58, 218);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (219, '2020/962932', 'sociis natoque penatibus et', 2818.0, 591.78, 46.45, 3409.78, 219);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (220, '2020/399808', 'adipiscing lorem vitae mattis nibh ligula nec sem', 2964.11, 622.46, 14.43, 3586.57, 220);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (221, '2020/600098', 'semper rutrum nulla nunc purus phasellus in', 2173.77, 456.49, 2.53, 2630.26, 221);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (222, '2020/763490', 'morbi vestibulum velit', 3062.04, 643.03, 69.47, 3705.07, 222);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (223, '2020/263562', 'lacinia eget tincidunt eget tempus', 1599.24, 335.84, 145.15, 1935.08, 223);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (224, '2020/047694', 'ut at dolor quis odio', 2251.84, 472.89, null, 2724.73, 224);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (225, '2020/850114', 'felis donec semper sapien a libero nam dui proin leo', 2112.25, 443.57, null, 2555.82, 225);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (226, '2020/649964', 'sit amet diam in magna bibendum', 1658.21, 348.22, null, 2006.43, 226);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (227, '2020/105943', 'potenti nullam porttitor', 1626.81, 341.63, null, 1968.44, 227);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (228, '2020/629442', 'blandit mi', 322.34, 67.69, null, 390.03, 228);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (229, '2020/602211', 'curabitur in libero ut massa volutpat convallis morbi odio odio', 1656.36, 347.84, null, 2004.2, 229);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (230, '2020/785205', 'at', 3153.95, 662.33, null, 3816.28, 230);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (231, '2020/003566', 'in congue etiam justo', 1857.55, 390.09, null, 2247.64, 231);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (232, '2020/047301', 'sollicitudin vitae consectetuer eget rutrum', 1785.54, 374.96, null, 2160.5, 232);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (233, '2020/218322', 'platea dictumst aliquam augue quam sollicitudin vitae', 1805.65, 379.19, 101.61, 2184.84, 233);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (234, '2020/590547', 'ultrices posuere cubilia curae', 325.8, 68.42, null, 394.22, 234);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (235, '2020/888044', 'quam sapien varius ut', 722.23, 151.67, null, 873.9, 235);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (236, '2020/559575', 'nulla facilisi cras non velit nec nisi', 2858.71, 600.33, null, 3459.04, 236);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (237, '2020/957705', 'ridiculus', 2089.04, 438.7, null, 2527.74, 237);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (238, '2020/755834', 'congue diam id', 3375.05, 708.76, null, 4083.81, 238);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (239, '2020/771320', 'lorem integer tincidunt ante vel ipsum praesent', 3373.2, 708.37, 131.58, 4081.57, 239);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (240, '2020/486892', 'ut erat curabitur', 3406.05, 715.27, null, 4121.32, 240);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (241, '2020/826578', 'orci luctus', 1417.7, 297.72, null, 1715.42, 241);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (242, '2020/714429', 'nulla sed accumsan felis ut', 954.53, 200.45, null, 1154.98, 242);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (243, '2020/774401', 'semper rutrum nulla nunc purus phasellus', 2028.76, 426.04, null, 2454.8, 243);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (244, '2020/244838', 'nam', 2809.01, 589.89, null, 3398.9, 244);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (245, '2020/357560', 'quam sollicitudin vitae consectetuer eget', 2069.24, 434.54, null, 2503.78, 245);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (246, '2020/761577', 'nulla justo aliquam quis turpis eget elit sodales', 838.81, 176.15, null, 1014.96, 246);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (247, '2020/833692', 'ipsum dolor sit amet consectetuer', 1243.32, 261.1, null, 1504.42, 247);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (248, '2020/590287', 'diam in', 455.79, 95.72, null, 551.51, 248);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (249, '2020/069073', 'nullam sit', 2417.82, 507.74, 70.76, 2925.56, 249);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (250, '2020/829589', 'lectus pellentesque eget nunc donec quis orci', 312.19, 65.56, 25.44, 377.75, 250);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (251, '2020/659587', 'viverra eget congue eget semper rutrum nulla nunc purus', 942.26, 197.87, null, 1140.13, 251);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (252, '2020/793774', 'mi integer ac neque duis', 1223.86, 257.01, null, 1480.87, 252);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (253, '2020/145919', 'adipiscing lorem vitae mattis nibh ligula', 2803.59, 588.75, null, 3392.34, 253);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (254, '2020/325045', 'massa', 550.87, 115.68, 133.08, 666.55, 254);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (255, '2020/615180', 'in faucibus orci luctus et ultrices posuere cubilia curae duis', 2190.25, 459.95, 52.56, 2650.2, 255);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (256, '2020/035092', 'lacus at turpis donec posuere metus vitae ipsum', 3425.48, 719.35, null, 4144.83, 256);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (257, '2020/711214', 'amet justo', 302.18, 63.46, 57.31, 365.64, 257);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (258, '2020/022824', 'vestibulum ante ipsum primis in faucibus orci luctus', 3368.73, 707.43, null, 4076.16, 258);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (259, '2020/004965', 'tempor convallis nulla neque libero convallis', 3102.02, 651.42, null, 3753.44, 259);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (260, '2020/277244', 'turpis sed ante', 686.59, 144.18, 81.04, 830.77, 260);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (261, '2020/420332', 'faucibus', 1343.59, 282.15, null, 1625.74, 261);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (262, '2020/029075', 'mauris non ligula pellentesque ultrices phasellus id sapien in sapien', 3174.98, 666.75, 123.13, 3841.73, 262);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (263, '2020/300366', 'amet lobortis sapien sapien non mi integer', 2211.29, 464.37, null, 2675.66, 263);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (264, '2020/615713', 'in tempus sit', 3441.29, 722.67, null, 4163.96, 264);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (265, '2020/791551', 'aliquet pulvinar', 2587.48, 543.37, 117.38, 3130.85, 265);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (266, '2020/477360', 'nulla integer pede', 2920.2, 613.24, null, 3533.44, 266);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (267, '2020/338577', 'luctus et ultrices', 2327.26, 488.72, 67.66, 2815.98, 267);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (268, '2020/956836', 'vivamus metus arcu adipiscing molestie hendrerit', 1709.6, 359.02, null, 2068.62, 268);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (269, '2020/323506', 'eu', 3097.13, 650.4, null, 3747.53, 269);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (270, '2020/696062', 'vel lectus in quam fringilla rhoncus mauris enim', 3018.68, 633.92, null, 3652.6, 270);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (271, '2020/441969', 'cum sociis natoque penatibus', 1921.98, 403.62, null, 2325.6, 271);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (272, '2020/571701', 'integer', 1203.94, 252.83, null, 1456.77, 272);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (273, '2020/901129', 'ante vestibulum ante ipsum primis in faucibus orci luctus et', 2232.38, 468.8, 36.51, 2701.18, 273);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (274, '2020/917482', 'erat vestibulum sed magna at nunc', 1734.11, 364.16, null, 2098.27, 274);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (275, '2020/466770', 'quisque erat eros viverra', 1988.48, 417.58, null, 2406.06, 275);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (276, '2020/145061', 'mi integer ac neque duis', 2897.64, 608.5, 95.69, 3506.14, 276);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (277, '2020/173470', 'ut rhoncus aliquet pulvinar sed nisl nunc', 3110.1, 653.12, 91.4, 3763.22, 277);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (278, '2020/081737', 'vehicula consequat morbi a ipsum', 1531.83, 321.68, 12.39, 1853.51, 278);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (279, '2020/629617', 'nibh in quis justo maecenas rhoncus aliquam lacus morbi', 2454.83, 515.51, 91.54, 2970.34, 279);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (280, '2020/499155', 'ac est lacinia', 3187.25, 669.32, null, 3856.57, 280);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (281, '2020/816858', 'primis', 1476.56, 310.08, null, 1786.64, 281);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (282, '2020/963494', 'curabitur in libero ut massa', 1130.08, 237.32, 48.24, 1367.4, 282);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (283, '2020/154839', 'praesent', 2585.36, 542.93, 86.42, 3128.29, 283);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (284, '2020/160151', 'eget', 3294.6, 691.87, null, 3986.47, 284);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (285, '2020/066939', 'porta volutpat erat quisque erat eros viverra', 1768.18, 371.32, null, 2139.5, 285);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (286, '2020/481939', 'odio curabitur convallis duis', 1370.44, 287.79, null, 1658.23, 286);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (287, '2020/704618', 'nascetur', 1258.0, 264.18, null, 1522.18, 287);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (288, '2020/702942', 'justo nec condimentum neque sapien placerat ante nulla justo', 311.64, 65.44, null, 377.08, 288);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (289, '2020/175429', 'sollicitudin vitae consectetuer eget rutrum at lorem integer tincidunt', 3481.59, 731.13, null, 4212.72, 289);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (290, '2020/117301', 'nisi vulputate nonummy maecenas tincidunt lacus at velit', 1555.37, 326.63, null, 1882.0, 290);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (291, '2020/159682', 'donec vitae nisi nam ultrices libero non mattis pulvinar', 439.42, 92.28, null, 531.7, 291);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (292, '2020/259848', 'proin at turpis', 1211.6, 254.44, null, 1466.04, 292);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (293, '2020/225528', 'nulla integer pede justo lacinia eget', 2508.17, 526.72, 33.25, 3034.89, 293);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (294, '2020/530727', 'volutpat eleifend donec ut dolor morbi', 2191.0, 460.11, null, 2651.11, 294);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (295, '2020/421947', 'quis augue luctus tincidunt', 2325.68, 488.39, 117.87, 2814.07, 295);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (296, '2020/899053', 'praesent blandit lacinia erat vestibulum sed magna at nunc', 1155.63, 242.68, null, 1398.31, 296);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (297, '2020/162805', 'aliquet pulvinar sed', 3489.22, 732.74, 32.09, 4221.96, 297);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (298, '2020/144120', 'non interdum in ante vestibulum ante ipsum primis in', 1642.74, 344.98, null, 1987.72, 298);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (299, '2020/158943', 'vestibulum', 2376.8, 499.13, null, 2875.93, 299);
insert into facturen (id, factuurnummer, beschrijving, prijs, btw, korting, totale_prijs, klant) values (300, '2020/571985', 'nec nisi vulputate nonummy maecenas tincidunt lacus at velit vivamus', 2653.45, 557.22, null, 3210.67, 300);

```

### bungalowpark
```
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (7, 'Ravenstraat', 481, 1813, 'Wilsele');
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (4, 'Urselweg', 246, 9104, 'Begijnendijk');
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (1, 'Urselweg', 1, 6861, 'Tienen');
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (4, 'Mussenstraat', 262, 3797, 'Begijnendijk');
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (3, 'Mussenstraat', 114, 7089, 'Geetbets');
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (2, 'Ravenstraat', 16, 6050, 'Knokke-Heist');
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (8, 'Urselweg', 404, 1809, 'Maldegem');
insert into bungalowpark (id, straat, huisnummer, postcode, gemeente) values (7, 'Bondgenotenlaan', 204, 6416, 'Tielt-Winge');

```
<!--stackedit_data:
eyJoaXN0b3J5IjpbODg1NTQzMTM0LDcwNjgxMDc3LC00OTUwNz
kxNDMsLTU0NDU4MDA4MywxODU0MzUyNDI5LDY2MzUzMjg5LC05
NTUyNDkxMDddfQ==
-->
