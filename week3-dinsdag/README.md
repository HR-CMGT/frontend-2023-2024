# Week 3 - Dinsdag

<br>

**Inhoudsopgave**

- [Week 3 - Dinsdag](#week-3---dinsdag)
  - [Opdracht 1 - Werkomgeving gereed maken](#opdracht-1---werkomgeving-gereed-maken)
    - [Opdracht 1a - Visual Studio Code installeren](#opdracht-1a---visual-studio-code-installeren)
    - [Opdracht 1b - Extensie Live Server installeren](#opdracht-1b---extensie-live-server-installeren)
    - [Opdracht 1c - Eerste project aanmaken](#opdracht-1c---eerste-project-aanmaken)
    - [Opdracht 1d - Bestandsstructuur HTML en CSS](#opdracht-1d---bestandsstructuur-html-en-css)
    - [Opdracht 1e - Code testen](#opdracht-1e---code-testen)
  - [Opdracht 2 - HTML](#opdracht-2---html)
  - [Opdracht 3 - Basisstructuur HTML](#opdracht-3---basisstructuur-html)
  - [Opdracht 4 - CSS](#opdracht-4---css)
  - [Opdracht 5 - Images](#opdracht-5---images)

<br><hr><br>

## Opdracht 1 - Werkomgeving gereed maken

Om te kunnen beginnen met programmeren heb je een app nodig waarin dit kan, ook wel
een [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment) genoemd. In onderstaande stappen installeer
je eerst `Visual Studio Code` en vervolgens de extensie `Live Server` en maak je je eerste project aan.

<br><br>

### Opdracht 1a - Visual Studio Code installeren

1. Ga naar https://code.visualstudio.com en klik op de download-knop;
2. Op een MacBook: open het gedownloade bestand en versleep de app naar de apps-map;
3. Op een Windows: open het gedownloade bestand en doorloop de stappen van de installatie met de standaard instellingen.

<br><br>

### Opdracht 1b - Extensie Live Server installeren

Om de door jou geschreven code te testen in de browser heb je een extensie nodig die dit mogelijk maakt,
genaamd `Live Server`. Hiermee worden wijzigingen die je in de code maakt direct zichtbaar in de browser. In deze
opdracht ga je de extensie alleen installeren, dus nog niet gebruiken, dat komt pas
bij [opdracht 1d](#opdracht-1d---bestandsstructuur-html-en-css).

1. Wanneer Visual Studio Code geopend is, klik je links op `Extensions` (het icoontje met vier blokjes);
2. Voer `Live Server` in de zoekbalk in en installeer de extensie (het is degene gemaakt door Ritwick Dey);

<br>

> De browser is een app op jouw laptap waarmee je websites bekijkt. Bekende browsers zijn Microsoft Edge, Google Chrome,
> Firefox en Safari.

<br><br>

### Opdracht 1c - Eerste project aanmaken

Voor ieder project waaraan je werkt maak je een nieuw project aan in Visual Studio Code. Je gaat nu jouw eerste project
aanmaken. Dit project kan je gedurende het vak gebruiken om de lesopdrachten te maken. Voor de eindopdracht van dit vak
maak je (op een later moment) weer een nieuw project aan.

1. Het aanmaken van een nieuw project is zo simpel als het aanmaken van een nieuwe map. Klik links boven
   op `File -> Open Folder...`;
2. Ga naar de map waar je dit project wilt neerzetten en maak daar een nieuwe map aan met de gewenste naam,
   bijvoorbeeld `frontend-development` (de naam mag geen spaties bevatten). Klik vervolgens op `Open`
   of `Map selecteren`;
3. Je hebt nu je eerste project aangemaakt!
4. Misschien krijg je een melding, klik dan op `Yes, I trust the authors`.

<br><br>

### Opdracht 1d - Bestandsstructuur HTML en CSS

Wanneer je met HTML en CSS werkt heb je altijd een bepaalde `bestandsstructuur` nodig van bestanden en mappen. Dat ga je
in deze opdracht aanmaken. Allereerst is het goed om te weten dat je door de lessen heen een aantal hoofdopdrachten
maakt. Iedere hoofdopdracht maak je in een eigen map, met daarin weer diezelfde bestandsstructuur die je in deze
opdracht gaat maken. Je gaat nu dus eerst een map voor de les van vandaag maken. Zorg ervoor dat links de `Explorer`
geopend is (icoontje met de twee A4'tjes). De benodigde knoppen om deze opdracht uit te voeren vind je aan de
linkerzijde, rechts van de projectnaam.

1. Maak een map aan met de naam `les1` (zonder spaties);
2. Maak in deze nieuwe map een bestand aan met de naam `index.html` en zet de basis-HTML neer door een `!` te typen en
   op de tab-toets te drukken;
3. Maak een map aan met de naam `css` en maak hierin een bestand aan met de naam `style.css`;
4. Koppel het CSS-bestand aan het HTML-bestand door de volgende regel aan de `<head>` in de `index.html` toe te voegen:

```html

<link rel="stylesheet" href="css/style.css">
```

5. Zorg ervoor dat de `bestandsstructuur` en de code van de `index.html` er als volgt uitzien:

<img  src="./images/Opdracht1.png" alt="Opdracht 1" title="Opdracht 1" width="1012"/>

<br><br>

### Opdracht 1e - Code testen

Het project is gereed en je bent klaar om te beginnen met programmeren! Om de door jou geschreven code te testen heb je
de extensie `Live Server` nodig (geïnstalleerd in [opdracht 1b](#opdracht-1b---extensie-live-server-installeren)). Met
de volgende stappen leer je hoe je deze extensie gebruikt.

1. Plaats eerst content in de `<body>`, bijvoorbeeld: `<h1>Hallo Wereld</h1>`
2. Klik met de rechter muistoets op `index.html` in de linker zijbalk en vervolgens op `Open with Live Server`.
3. Het document wordt nu geopend in de browser en je zou de heading `Hallo wereld` moeten zien.
4. Wanneer je iets wijzigt in je code en het bestand opslaat wordt dit automatisch bijgewerkt in de browser. Pas de h1
   maar eens aan naar: `<h1>Hallo wereld, mijn naam is [JOUW NAAM]</h1>` en sla het bestand op (MacBook: CMD+S /
   Windows: CTRL+S). Wanneer je de browser opent zie je als het goed is dat deze wijziging direct zichtbaar is.

> Je hoeft dus niet telkens opnieuw de `live server` te starten!

<br><hr><br>

> ⚠️ Opdracht 2 t/m 5 maak je in de bestanden die je bij [opdracht 1d](#opdracht-1d---bestandsstructuur-html-en-css)
> hebt gemaakt.

<br>

## Opdracht 2 - HTML

Bouw het volgende ontwerp na *(klik op de afbeelding om te vergroten)*.
<br>
In de tabel hieronder zie je welke HTML-tags je nodig hebt voor deze opdracht.

> Als bonus mag je de navigatielinkjes bovenin werkend maken, maar dit is niet vereist voor deze opdracht.

<img src="./images/Opdracht2.png" alt="Opdracht 2" title="Opdracht 2" width="1012">

<br>


Je hebt hier het volgende voor nodig:

| HTML | CSS | Gebruikte kleuren |
|------|-----|-------------------|
| h1   | -   | -                 |
| h2   |     |                   |
| p    |     |                   |
| a    |     |                   |

<br>

> ### Dummy text
>
> Bij het maken van je website kan het nodig zijn om alvast **dummy tekst** te plaatsen, om te zien of je layout goed
> werkt. Je kan hier [lorum ipsum tekst](https://www.google.nl/search?q=lorum+ipsum "Google op lorum ipsum")
> of [ChatGPT](https://chat.openai.com) voor gebruiken.

<br>

**Hulpbronnen opdracht 2**

1. [Introductievideo HTML & CSS](https://www.youtube.com/watch?v=0sQLdlAodfQ "Introductievideo HTML & CSS")
2. [Introductievideo HTML](https://www.youtube.com/watch?v=apC46Wfvd94 "Introductievideo HTML") (*bekijk tot 04:33, het
   deel erna is niet van toepassing voor dit vak*)

<br><hr><br>

## Opdracht 3 - Basisstructuur HTML

Nu je de tekstuele elementen in de vorige opdracht hebt aangemaakt, wordt het tijd om hier structuur in aan te brengen
met semantische tags. Zoals je in onderstaand ontwerp ziet, zal na deze opdracht de pagina visueel nog niet veranderd
zijn, maar op de achtergrond heb je essentiële stappen genomen.
In de tabel hieronder zie je welke HTML-tags je nodig hebt voor deze opdracht.

<img src="./images/Opdracht3.png" alt="Opdracht 3" title="Opdracht 3" width="1012">

<br>
Je hebt hier het volgende voor nodig:

| HTML    | CSS | Gebruikte kleuren |
|---------|-----|-------------------|
| header  | -   | -                 |
| main    |     |                   |
| footer  |     |                   |
| nav     |     |                   |
| section |     |                   |
| div |     |                   |

<br>

**Hulpbronnen opdracht 3**

1. [Instructie CMGT-dag over structuur aanbrengen](https://www.youtube.com/watch?v=h042V7L6NXM&t=160s) (*de video start
   op 02:40, bekijk tot 08:00, de rest is niet van toepassing voor deze opdracht*)
2. [HTML cheatsheet](./images/HTML-cheatsheet.png  )
3. [Wireframe basisstructuur HTML](./images/Basisstructuur-HTML.jpg  )

<br><hr><br>

## Opdracht 4 - CSS

Bouw het volgende ontwerp na *(klik op de afbeelding om te vergroten)*.
<br>
De HTML van de pagina staat nu volledig, dus het wordt tijd om hier styling aan te geven met CSS. In de tabel hieronder zie je wat je nodig hebt in de CSS voor deze opdracht.

<img src="./images/Opdracht4.png" alt="Opdracht 4" title="Opdracht 4" width="1012">

<br>

Je hebt hier het volgende voor nodig:

| HTML | CSS                    | Gebruikte kleuren |
|------|------------------------|-------------------|
| -    | Selecting o.b.v. tag   | #717D96           |
|      | Selecting o.b.v. class | #A0ABC0           |
|      | font-family            | #E2E7F0           |
|      | color                  | #4A5468           |
|      | background-color       | #FFFFFF           |
|      | text-align             |                   |

<br>

**Hulpbronnen opdracht 4**

1. [CSS cheatsheet](./images/CSS-cheatsheet.png)
2. [Introductievideo CSS](https://www.youtube.com/watch?v=apC46Wfvd94 "Introductievideo CSS") (*bekijk tot 11:00, het
   deel erna is niet van toepassing voor dit vak*)

<br><hr><br>

## Opdracht 5 - Images

Voeg één of meerdere afbeeldingen toe aan jouw pagina. Je mag zelf bepalen welke afbeeldingen je voor deze oefening gebruikt en waar je ze op de pagina toevoegt. Dit werkt iets anders dan je gewend bent in Codepen. Je zult de afbeelding namelijk eerst moeten opslaan in de projectmap, om die vervolgens in te laden in de HTML. Doorloop de volgende stappen:

1. Maak in de map `week3-les1` een nieuwe map aan met de naam `images`;
2. Plaats in deze nieuwe map jouw afbeelding(en);
3. Voer tot slot de afbeelding(en) in de HTML in met de volgende code (vervang de placeholders):

```html
<img src="images/[NAAM_EN_EXTENSIE_BESTAND]" alt="[ALTERNATIEVE_TEKST]">
```

Zoals je kunt zien gebruik je hier als `src` niet de gehele url (zoals wel nodig was in Codepen), maar je voert
het `pad naar de afbeelding` in vanaf de `index.html` gezien. Dit noem je een `relatief pad`. Dus stel, de bestandsnaam
van jouw afbeelding is `profielfoto.jpg`, dan is het relatieve pad dat je moet invoeren `images/profielfoto.jpg`.
