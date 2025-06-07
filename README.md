# Alle Nederlandse adressen en bijbehorende postcodes

![Adressen](https://img.shields.io/badge/adressen-9.641.805-brightgreen) ![Laatste update](https://img.shields.io/badge/laatste%20update-07--06--2025-brightgreen)

<a href="https://www.buymeacoffee.com/Lars-" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-orange.png" alt="Buy Me A Coffee" height="60" style="height: 60px !important;width: 217px !important;" ></a>

Deze repository bevat alle Nederlandse adressen, bijbehorende postcodes, coordinaten en andere belangrijke gegevens om jouw tijd en geld te besparen.

## Why Dutch?

This readme is in Dutch (except this part) because the content is based on Dutch data. We cannot imagine that anyone outside the Netherlands would need this data. If they do, please let us know. Even with this Dutch readme, we think
everyone will understand how it works.

## Doel

Een abonnement op postcodediensten is vaak duur, terwijl deze informatie gratis beschikbaar is bij overheidsinstanties. Helaas verstrekken zij niet één groot bestand met alle informatie, en daar maken bedrijven graag gebruik van.

In deze repository vind je alle gegevens die je nodig hebt om adressen naar postcodes om te zetten en vice versa.

## Inhoud

Alles is ingepakt in .tar.xz bestanden om ruimte te besparen. We besparen hier gemiddeld 95% schijfruimte mee.

- adressen.tar.xz (1.0GB uitgepakt): dit archief bevat een CSV-bestand met daarin van alle adressen de volgende gegevens:
    - Straatnaam
    - Huisnummer
    - Postcode
    - Woonplaatsnaam
    - Gemeentenaam
    - Provincienaam
    - Latitude
    - Longitude
- provincies.tar.xz (931.8MB uitgepakt): dit archief bevat CSV-bestanden van alle adressen, gesplitst per provincie.

Het CSV-bestand kan geïmporteerd worden in phpMyAdmin (o.i.d.) om het vervolgens in je applicatie te gebruiken.

Deze repository heeft altijd slechts één commit. Bij elke update wordt de data overschreven. Versiebeheer werkt niet bij gecomprimeerde bestanden, dus het bewaren van elke versie is niet zinvol en zorgt alleen voor lange wachttijden bij het
clonen of pullen van deze repository.

## Actualiteit en betrouwbaarheid

We streven ernaar om elke week een bijgewerkte versie te pushen. Bovenaan deze readme zie je wanneer de laatste update heeft plaatsgevonden.

De data die we aanbieden wordt, voor zover wij weten, ook gebruikt door overheidsinstanties zoals het Kadaster. We verwachten dus dat de data 100% betrouwbaar is. Als er toch fouten zijn, laat het ons dan weten.

## Maatwerk

Geïnteresseerd in maatwerk op basis van deze gegevens of iets anders? Neem dan contact op
via [info@ljpc.nl](mailto:info@ljpc.nl?subject=Postcode%20repository).

## Doneren

Als we je zojuist een hoop tijd en geld bespaard hebben, zouden we het fijn vinden als je zou willen overwegen een
donatie te doen. Alle donaties worden gebruikt om systemen als dit mogelijk te
maken. [Klik hier](https://www.buymeacoffee.com/Lars-) om te doneren.
