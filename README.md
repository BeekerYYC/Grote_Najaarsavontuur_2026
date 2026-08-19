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
- `.nojekyll` — zodat GitHub Pages het bestand ongewijzigd serveert.

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
