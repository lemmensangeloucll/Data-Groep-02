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

3. Welk bungalowtype werd al meer dan 50 keer gekozen bij reservaties voor het bungalowpark in de Ravenstraat 1813 
en hoevaak wordt het er precies gekozen?





4. Geef het aantal klanten hen hun gemeente waarvan de gemeente van het bungalowpark waar ze reserveren niet hetzelfde is.

Reden: Zo kan de eigenaar van een bungalowpark een idee hebben of de mensen van verder weg ook weet hebben over het bestaan van het bungalowpark.



3. Geef het gemiddelde van de totale prijs van alle facturen die door de klanten worden betaald.

Reden: Zo kan mn een idee hebben wat een klant gemiddeld betaald na een bezoekje aan een bungalowpark



4. Geef het totaal aantal reservaties die in de zomer gedaan worden waarbij er meer dan 2 extra activiteiten zijn gekozen.

Reden: Zo heeft mn zicht op de werknemers(eventueel vakantiejobbers)die mn nodig zal hebben in de zomer om de activiteiten te hosten.


5. GEZOCHT


#Geef het aantal klanten dat een annulatieverzekering neemt maar deze achteraf heeft geannuleerd
