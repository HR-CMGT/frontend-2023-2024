# Quiz - Semantische HTML

Dit is een quiz over semantische HTML.
<br>
Noteer voor jezelf het antwoord per vraag. Later deze les worden de antwoorden online gezet. Vergelijk dan zelf jouw antwoorden met het antwoordmodel.
<br><br>

>Vul deze quiz in zo vaak als je wilt, het liefst totdat je geen fouten meer maakt.

<br><hr><br>

## Vraag 1

Geef aan of de volgende stelling klopt: In onderstaande HTML moet op regel 3 en 6 `<div>` naar `<section>` worden omgezet.

```html
1.  <main>
2.      <section id="introduction">
3.          <div class="left-column">
4.              <h1>Welkom op mijn website</h1>
5.          </div>
6.          <div class="right-column">
7.              <p>Mijn naam is...</p>
8.          </div>
9.      </section>
10. </main>
```

A. Waar
<br>
B. Niet waar

<br><hr><br>

## Vraag 2

Wat is semantisch gezien incorrect in de volgende HTML?
<br>*Meerdere antwoorden mogelijk.*

```html
1.  <header>
2.      <nav>
3.          <a href="#introduction">Introductie</a>
4.      </nav>
5.  </header>
6.  
7.  <section>
8.      <div id="introduction">
9.          <h1>Welkom op mijn website</h1>
10.         <p>Mijn naam is...</p>
11.     </div>
12. </section>
```

A. De `<nav>` mag niet in de `<header>` staan
<br>
B. De `<div>` op regel 8 moet een `<section>` zijn
<br>
C. De `<h1>` moet altijd in de `<header>` staan
<br>
D. De id moet ingesteld staan op de `<h1>` in plaats van de `<div>`
<br>
E. De `<section>` op regel 7 moet in een `<main>` worden geplaatst.
