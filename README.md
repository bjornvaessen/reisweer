# Reisweer

Een reisplanner die het weer voor je hele rondreis in één overzicht laat zien, zonder te
schakelen tussen aparte plekken in je weer-apps.

## Waarom

Bij een rondreis met meerdere stops kost het uitzoeken van het weer per plaats behoorlijk wat tijd. Reisweer zet je route neer als een tijdlijn: elke stop met
bijbehorende data, en het weer voor precies die dagen waarop je er bent.

## Functies

- **Meerdere reisplannen**, elk met een reeks stops in volgorde
- **Automatische startdatum**: een nieuwe stop begint waar de vorige eindigt
- **Weer per stop**, met een duidelijk onderscheid tussen een harde voorspelling en een
  langjarig gemiddelde (gemarkeerd met `~`) voor dagen ver vooruit
- **Dagdetails met één klik**: UV-index, neerslag in mm, gevoelstemperatuur, wind, zonsopkomst
  en -ondergang, en — bij Visual Crossing — ook luchtvochtigheid, luchtdruk, zicht, bewolking
  en maanfase. Inclusief een uurgrafiek van temperatuur en neerslagkans, met een eigen as voor
  elk van de twee.
- **Blader door de hele reis**: klik door alle dagen van de reis vanuit het dagdetail
- **Twee weerdiensten om uit te kiezen** (via Instellingen):
  - [Open-Meteo](https://open-meteo.com): gratis, geen sleutel nodig, tot ~16 dagen vooruit
  - [Visual Crossing](https://www.visualcrossing.com): eigen gratis sleutel nodig, kijkt
    verder vooruit via statistische gemiddelden. De sleutel wordt alleen lokaal in je browser
    bewaard.
- **Luchtkwaliteit en brandhaarden** (via Instellingen): luchtkwaliteit (Open-Meteo, 7 dagen vooruit) en brandhaarden binnen een straal van 60 kilometer van de stop (NASA FIRMS, gratis sleutel nodig)
- **Bekijk- en bewerkmodus**: een opgeruimd overzicht om te bekijken, een aparte bewerkmodus
  (potlood-icoon) om een reisplan aan te passen
- **Bewaren & laden**: reisplannen als bestand downloaden of als tekst kopiëren, zodat je ze
  kunt meenemen naar een andere browser of computer
- **Prettig op telefoon én desktop**: op mobiel staan de dagen onder elkaar als brede balken, op een groter scherm naast elkaar als tegels

## Gebruiken

De app staat live op GitHub Pages, direct te gebruiken zonder iets te downloaden:

**[bjornvaessen.github.io/reisweer](https://bjornvaessen.github.io/reisweer/)**

Je gegevens blijven lokaal in je browser (`localStorage`) — er is geen backend en er wordt
niets naar een server van Reisweer gestuurd. Voor het zoeken van plaatsen en het ophalen van
het weer is een actieve internetverbinding nodig.

## Techniek

- Gegenereerd met Claude
- Uitsluitend HTML, CSS en JavaScript. Geen frameworks, geen dependencies om te installeren
- Lettertypen (IBM Plex) worden geladen via Google Fonts
- Weerdata via [Open-Meteo](https://open-meteo.com) en optioneel
  [Visual Crossing](https://www.visualcrossing.com)
- Luchtkwaliteit via [Open-Meteo](https://open-meteo.com)
- Brandhaarden via [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/)

## Licentie

[GNU GPLv3](LICENSE)
