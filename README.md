# Het Grote Najaarsavontuur 2026 🚐

Reisgids-website voor de camper-rondreis van André & Tineke door Italië, najaar 2026.
Ruim 7.000 km: Bennekom → Luxemburg → Bodensee/Allgäu → Reschenpas → Stelvio → Sardinië →
Amalfikust & Cilento → Sicilië → Matera & Puglia → San Marino → Ravenna → Gardameer → Bennekom.
Camper inleveren bij CVD Driel op 16 oktober 2026.

De inhoud komt uit het originele reisboek (Word/PDF). Daarnaast staan er blauwe kaders in de
pagina met **extra suggesties uit online onderzoek** (augustus 2026), elk met bronvermelding —
bijvoorbeeld het Autunno in Barbagia-festival in Dorgali op 26–27 september, het camperverbod op
de SS163, de ZTL-camera's, en de olijfoogst bij Ostuni.

## Wat er in zit

- `index.html` — de complete website. Eén bestand, geen build, geen dependencies.
  Werkt in lichte en donkere modus en op mobiel.
- `img/` — 21 sfeerfoto's, verdeeld over de acht etappes (twee tot drie per deel).
  Allemaal van Wikimedia Commons en vrij te gebruiken (Creative Commons of CC0);
  fotograaf en licentie staan in de bijschriften, en de foto zelf linkt naar de
  bestandspagina op Commons. Opgeslagen als JPEG van 1200 px breed (samen ±4,5 MB)
  en met `loading="lazy"`, dus de browser haalt alleen op wat je ook echt bekijkt.
- `.nojekyll` — zodat GitHub Pages de bestanden ongewijzigd serveert.

## Publiceren via GitHub Pages

1. Push deze bestanden naar de `main`-branch van de repository.
2. Ga naar **Settings → Pages**.
3. Zet **Source** op `Deploy from a branch`, kies branch `main` en map `/ (root)`.
4. Na een minuut staat de site op `https://<gebruikersnaam>.github.io/<repo-naam>/`.

## Publiceren via Vercel

Importeer de repository in Vercel en laat alle instellingen op de standaardwaarden staan —
er is geen framework en geen buildstap nodig. Vercel serveert `index.html` direct.

## Aanpassen

Alles zit in dat ene HTML-bestand: de kleuren en fonts bovenaan in het `<style>`-blok
(als CSS-variabelen), daaronder de zeven etappes als `<section class="stage">`.
Een plaats toevoegen is een `<article class="place">` bijplakken; een tip toevoegen
een `<div class="tip">`.

Een foto toevoegen gaat net zo: zet het bestand in `img/` en plak een
`<figure class="shot">` bij in de `<div class="gallery">` van die etappe. De galerij
schaalt zelf mee — drie foto's naast elkaar op een breed scherm, twee op een tablet,
één op de telefoon. Vermeld in het bijschrift altijd fotograaf en licentie, en laat de
foto linken naar de bronpagina; dat is bij Creative Commons-foto's ook verplicht.
