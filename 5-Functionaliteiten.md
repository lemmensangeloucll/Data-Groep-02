## Functionaltieten

KLAAR:

1. Geef het bungalownummer en de beschikbaarheid van alle bungalows in het bungalowpark met
poscode XXXX die nog niet gereserveerd zijn en die geen reparatieaanvraag hebben

Reden: Zo kan een klant bijvoorbeeld aanvragen of er in het dichtsbijzijnde bugalowpark nog een plaats is.

#### Mogelijke oplossing - Gecontroleerd door: Angelo

```
select bungalownummer, beschikbaarheid from bungalow
inner join bungalowpark on bungalow.bungalowpark = bungalowpark.id
left join reparatie_aanvragen on bungalow.bungalownummer = reparatie_aanvragen.bungalow
where bungalowpark.postcode = '6861' and bungalow.beschikbaarheid = 'true' and reparatie_aanvragen.afgehandeld = 'true'
group by bungalownummer, beschikbaarheid
```

2. Geef het reservatiennummer, datum en naam van het bungalowpark id van alle reservaties die na 10/06/2019 en voor 10/09/2019 gemaakt zijn.

Reden: Zo kan de uitbater van een bungalowpark nagaan hoe druk de zomer ongeveer zal zijn of was tussen een bepaalde periode.

```
select reservatienummer, datum, bungalowpark.id
from reservaties 
full outer join bungalowpark on reservaties.bungalowpark = bungalowpark.id
where reservaties.datum >= '2019-06-10'  and reservaties.datum <= '2019-09-10' 
```

3. Welk bungalowtype werd al meer dan 10 keer gekozen bij reservaties voor het bungalowpark in Maldegem 
en hoevaak wordt het er precies gekozen?
```
select bungalowtype.klasse, count(reservaties.bungalowtype)
from reservaties 
inner join bungalowtype on reservaties.bungalowtype = bungalowtype.id
inner join bungalowpark on reservaties.bungalowpark = bungalowpark.id
where bungalowpark.gemeente = 'Maldegem'
group by bungalowtype.klasse
having count(bungalowtype.id) > 10
```



4. Geef het aantal reservaties waarvan de klanten hun gemeente niet hetzelfde is als de gemeente van het bungalowpark.

Reden: Zo kan de eigenaar van een bungalowpark een idee hebben of de mensen van verder weg ook weet hebben over het bestaan van het bungalowpark. Zo niet kan de eigenaar wat meer reclame op verdere plaatsen voorzien.





5. Geef de 4 meest gekozen faciliteiten bij een reservatie waarbij de klant geen annuleringsverzekering heeft genomen.

Reden: Zo weet de manager of de prijs van deze faciliteit moet stijgen of dalen en of dat er meer personeel moet worden voorzien voor deze faciliteit.



