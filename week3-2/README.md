# Week 3 les 2

<br>

**Inhoudsopgave**
<!-- TOC -->
- [Week 3 les 2](#week-3-les-2)
  - [Semantiek](#semantiek)
  - [Quiz over semantische HTML](#quiz-over-semantische-html)
  - [Werken met de inspector](#werken-met-de-inspector)
  - [Mini-oefeningen - Padding \& margin](#mini-oefeningen---padding--margin)
  - [Relatieve units](#relatieve-units)
  - [Opdrachten](#opdrachten)
<!-- TOC -->

<br><hr><br>

## Semantiek
AANTEKENING: Je mag HTML ***nooit*** gebruiken om een element in de gewenste stijl te krijgen. Dit doe je altijd met CSS. Dus niet `<strong>` gebruiken, omdat het dan dikgedrukt wordt, gebruik het vanwege de semantische betekenis.

<br>

**Veelgebruikte semantische tags voor structuur**
| Tag     | Omschrijving                                                                            |
| ------- | --------------------------------------------------------------------------------------- |
| header  | De header (bovenkant) van de pagina.                                                    |
| main    | De hoofdinhoud van de pagina.                                                           |
| footer  | De footer (onderkant) van de pagina.                                                    |
| nav     | Bevat de navigatie van de website.                                                      |
| section | Is om één sectie van de pagina aan te duiden.                                           |
| article | Is voor onafhankelijke, op zichzelf staande inhoud, zoals nieuwsberichten en blogposts. |

<br>

**Veelgebruikte semantische tags voor content**
| Tag    | Omschrijving                                                                           | Voorbeeld in HTML                                                                                                         | Eindresultaat                                                                                   |
| ------ | -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| strong | Nadruk leggen op een gedeelte van de tekst, omdat deze belangrijk of urgent is.        | `<p>`Before entering, he read the warning at the entrance: `<strong>`Caution! Fire-breathing dragon ahead.`</strong></p>` | Before entering, he read the warning at the entrance: **Caution! Fire-breathing dragon ahead.** |
| em     | Wanneer je op een gedeelte van de tekst verbaal de nadruk wilt leggen, vaak één woord. | `<p>`This will be `<em>`very`</em>` dangerous.`</p>`                                                                      | This will be *very* dangerous.                                                                  |


<br><hr><br>

## Quiz over semantische HTML
[Klik hier om de quiz over semantische HTML te doen](./quiz/)

<br><hr><br>

## Werken met de inspector

- Open de inspector op een specifiek HTML-element door met de rechter muistoets op dat element te klikken en vervolgens op **Inspecteren**;
  - Ook is de inspector te openen met de sneltoets ⌥⌘i op Mac en F12 op Windows;
- Van het geselecteerde element zie je ook alle bijbehorende CSS staan. Deze CSS is in de inspector aan te passen en dit is dan direct zichtbaar in de browser. Zo kan je spelen met de waardes en real-time wijzingen zien om het ontwerp te bepalen. Dit noemen we `Designing in the browser`;
  -  **Let op:** wanneer je CSS in de inspector wijzigt, verandert het ***niet*** in de bestanden in Visual Studio Code. Dit moet je handmatig wijzigen;

<img src="./images/designing.png" alt="Inspector" title="Inspector" width="800">

<br><hr><br>

## Mini-oefeningen - Padding & margin

[Klik hier om de naar de mini-oefeningen te gaan.](./mini-oefeningen/padding-margin)

<br><hr><br>

## Relatieve units

⚠️⚠️⚠️ **@TODO** maak cheatsheet over relatieve units ⚠️⚠️⚠️

<br><hr><br>


## Opdrachten

[Klik hier om de naar de opdrachten van deze les te gaan.](./opdrachten/)