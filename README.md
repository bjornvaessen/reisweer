# Reisweer

Een reisplanner die het weer voor je hele rondreis in één overzicht laat zien — zonder te
schakelen tussen aparte weer-apps per stad.

## Waarom

Bij een rondreis met meerdere stops kost het uitzoeken van het weer per plaats al snel meer
tijd dan de reis zelf plannen. Reisweer zet je route neer als een tijdlijn: elke stop met
bijbehorende data, en het weer voor precies die dagen ernaast.

## Functies

- **Meerdere reisplannen**, elk met een reeks stops in volgorde
- **Automatische startdatum**: een nieuwe stop begint waar de vorige eindigt
- **Weer per stop**, met een duidelijk onderscheid tussen een harde voorspelling en een
  langjarig gemiddelde (gemarkeerd met `~`) voor dagen ver vooruit
- **Twee weerdiensten om uit te kiezen** (via Instellingen):
  - [Open-Meteo](https://open-meteo.com): gratis, geen sleutel nodig, tot ~16 dagen vooruit
  - [Visual Crossing](https://www.visualcrossing.com): eigen gratis sleutel nodig, kijkt
    verder vooruit via statistische gemiddelden. De sleutel wordt alleen lokaal in je browser
    bewaard.
- **Bekijk- en bewerkmodus**: een opgeruimd overzicht om te bekijken, een aparte bewerkmodus
  (potlood-icoon) om een reisplan aan te passen
- **Bewaren & laden**: reisplannen als bestand downloaden of als tekst kopiëren, zodat je ze
  kunt meenemen naar een andere browser of computer

## Gebruiken

De app staat live op GitHub Pages, direct te gebruiken zonder iets te downloaden:

**[bjornvaessen.github.io/reisweer](https://bjornvaessen.github.io/reisweer/)**

Je gegevens blijven lokaal in je browser (`localStorage`) — er is geen backend en er wordt
niets naar een server van Reisweer gestuurd. Voor het zoeken van plaatsen en het ophalen van
het weer is een actieve internetverbinding nodig.

## Techniek

- Puur HTML, CSS en JavaScript; geen frameworks, geen dependencies om te installeren
- Lettertypen (IBM Plex) worden geladen via Google Fonts
- Weerdata via [Open-Meteo](https://open-meteo.com) en optioneel
  [Visual Crossing](https://www.visualcrossing.com)

## Licentie

[GNU GPLv3](LICENSE)
