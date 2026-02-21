# Alle Nederlandse adressen en bijbehorende postcodes

![Adressen](https://img.shields.io/badge/adressen-9.945.502-brightgreen) ![Laatste update](https://img.shields.io/badge/laatste%20update-21--02--2026-brightgreen)

<a href="https://www.buymeacoffee.com/Lars-" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-orange.png" alt="Buy Me A Coffee" height="60" style="height: 60px !important;width: 217px !important;" ></a>

Deze repository bevat alle Nederlandse adressen, bijbehorende postcodes, coördinaten en andere belangrijke gegevens.

## Why Dutch?

This readme is in Dutch (except this part) because the content is based on Dutch data. We cannot imagine that anyone outside the Netherlands would need this data. If they do, please let us know. Even with this Dutch readme, we think everyone will understand how it works.

## Doel

Een abonnement op postcodediensten is vaak duur, terwijl deze informatie gratis beschikbaar is bij overheidsinstanties. Helaas verstrekken zij niet één groot bestand met alle informatie, en daar maken bedrijven graag gebruik van.

In deze repository vind je alle gegevens die je nodig hebt om adressen naar postcodes om te zetten en vice versa.

## Inhoud

Alles is ingepakt in .zst-bestanden (Zstandard compressie) om ruimte te besparen. We besparen hier gemiddeld 85-90% schijfruimte mee.

- **Nederland.csv.zst** (72M gecomprimeerd, ~1.4GB uitgepakt): dit archief bevat een CSV-bestand met alle Nederlandse adressen en de volgende gegevens:
    - Straatnaam
    - Huisnummer
    - Huisletter
    - Huisnummertoevoeging
    - Postcode
    - Woonplaatsnaam
    - Gemeentenaam
    - Provincienaam
    - Latitude (WGS84)
    - Longitude (WGS84)

- **Provinciebestanden** (12 bestanden): CSV-bestanden van alle adressen, gesplitst per provincie:
    - Drenthe.csv.zst
    - Flevoland.csv.zst
    - Friesland.csv.zst
    - Gelderland.csv.zst
    - Groningen.csv.zst
    - Limburg.csv.zst
    - Noord-Brabant.csv.zst
    - Noord-Holland.csv.zst
    - Overijssel.csv.zst
    - Utrecht.csv.zst
    - Zeeland.csv.zst
    - Zuid-Holland.csv.zst

### CSV-formaat

De CSV-bestanden gebruiken **puntkomma (;)** als scheidingsteken en UTF-8 encoding.

**Headers:**
```
straat;huisnummer;huisletter;huisnummertoevoeging;postcode;woonplaats;gemeente;provincie;lat;lon
```

**Voorbeeld:**
```
De Ruijterkade;99;;;1011AB;Amsterdam;Amsterdam;Noord-Holland;52.3786674;4.90544356
Kalverstraat;1;A;;1012NZ;Amsterdam;Amsterdam;Noord-Holland;52.37123456;4.89165432
```

## Technische details

- **Coördinatensysteem:** WGS84 (EPSG:4326) - standaard GPS coördinaten
- **Compressie:** Zstandard (zstd) met maximum compressie (--ultra -22)
- **CSV delimiter:** Puntkomma (;)
- **Encoding:** UTF-8

## Veelgestelde vragen

**Q: Waarom .zst-bestanden en niet .zip of .tar.gz?**
A: Zstandard biedt betere compressie (85-90% vs 75-80% bij gzip) en is veel sneller bij uitpakken. Moderne tools ondersteunen het goed.

**Q: Kan ik de data commercieel gebruiken?**
A: Ja, de data heeft een CC0 licentie (publiek domein). Er zijn geen restricties.

**Q: Zijn de coördinaten nauwkeurig?**
A: Ja, de coördinaten komen van het Kadaster en zijn afgerond op 8 decimalen (~1mm nauwkeurigheid).

## Maatwerk

Geïnteresseerd in maatwerk op basis van deze gegevens of iets anders? Neem dan contact op
via [info@ljpc.nl](mailto:info@ljpc.nl?subject=Postcode%20repository).

## Gratis Postcodedata API

Wil je deze data niet zelf hosten? Gebruik dan onze gratis API op [gratis-postcodedata.nl](https://gratis-postcodedata.nl) — een gratis alternatief voor commerciële diensten zoals PostcodeAPI.nu en Pro6PP.

### API Gebruik

```bash
# Geen registratie of API key nodig
curl "https://gratis-postcodedata.nl/api/postcode/1012AB/1"
```

**Kenmerken:**
- 9+ miljoen Nederlandse adressen
- 470.000+ unieke postcodes
- Inclusief straat, woonplaats, gemeente, provincie en GPS-coördinaten
- Rate limit: 60 requests/minuut per IP
- Responstijd: <50ms
- OpenAPI specificatie: `/api/openapi.json`

### Wanneer wat gebruiken?

| Toepassing | Aanbevolen |
|------------|------------|
| Real-time adresvalidatie | gratis-postcodedata.nl API |
| Bulk verwerking/analyse | Deze CSV bestanden |
| Offline/zelf hosten | Deze CSV bestanden |
| Simpele postcode lookup | gratis-postcodedata.nl API |

## Doneren

Als we je zojuist een hoop tijd en geld bespaard hebben, zouden we het fijn vinden als je zou willen overwegen een
donatie te doen. Alle donaties worden gebruikt om systemen als dit mogelijk te maken.

<a href="https://www.buymeacoffee.com/Lars-" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-orange.png" alt="Buy Me A Coffee" height="60" style="height: 60px !important;width: 217px !important;" ></a>
