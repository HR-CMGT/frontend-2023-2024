# Week 6 - Dinsdag

- Transform, 3D, filter
- Transition
- Animation
- Position fixed
- Oefening

<br><br><br>

## Transform, 3D, filter

Met transform kan je een element schalen, roteren of verplaatsen, zonder dat je layout verstoord wordt. Dit werkt vaak goed samen met `hover` effecten en animaties. Als je meerdere transforms wil combineren moet je die samen op 1 regel plaatsen. Met `translate` verplaats je het element op de x,y as. Met `transform-origin` bepaal je het middelpunt van de transform.

```css
div {
    transform:scale(2) rotate(10deg) translate(10px, 10px);
    transform-origin:center; 
}
```

### 3D Effect

Je kan elementen roteren op een 3D as, met `rotateX`, `rotateY`, `rotateZ`. Je moet de parent container een `perspective` waarde geven, dit is de afstand van het element tot de gebruiker.

```css
.parent {
    perspective:100px;
}
.child {
    rotateY:20deg;
}
```

<br>

### Filter

Er zijn verschillende [filters](https://developer.mozilla.org/en-US/docs/Web/CSS/filter-function) beschikbaar die je op je elementen kan loslaten. Deze filters werken goed samen met transitions en animations. 

```css
div {
  filter: blur(20px) brightness(50%) saturate(4) hue-rotate(24deg);
}
```

<br><br><br>

## Transition

Een *transition* is een *animatie* die automatisch afspeelt op het moment dat de CSS van een element verandert. Dit werkt goed samen met `hover` effecten. Je kan bijna alle eigenschappen animeren, zoals:
  - kleur,
  - afmeting,
  - transform,
  - margin, padding
  - box-shadow,
  - css filter

In dit voorbeeld komt een kaartje los van de ondergrond on mouse hover.

```css
.card {
     color:white;
     background-color:lightgrey;
     transform-origin:center;
     transition: all 1s ease;
}
.card:hover {
    color:black;
    background-color:darkgrey;
    box-shadow: 5px 5px 10px rgb(0 0 0 / 0.4);
    transform:scale(1.2);  
}
```

<br><br><br>

## Animation

Een animatie kan je laten afspelen tussen twee of meer keyframes. De animatie kan automatisch afspelen, en je kan meerdere complexe animaties na elkaar laten afspelen. Om te beginnen bepaal je met CSS `@keyframes` welke eigenschappen gaan animeren. 

```css
@keyframes my-cool-animation {
  from {
    opacity:0;
    transform: translateX(20%);
  }
  to {
    opacity:1;
    transform: translateX(0%);
  }
}
```
Vervolgens kan je de keyframes toekennen aan een element via het `animation` keyword. Hierin kan je ook aangeven hoe lang de animatie duurt, of het moet herhalen, etc.
```css
div {
    animation: 3s ease-in infinite my-cool-animation;
}
```


> De browser inspector heeft een [animation inspector](https://youtu.be/w4J8sJpHKvw?si=NnAbrkcKg81YJfFA) om de timing van je animaties mee te ontwerpen.

<br><br><br>

## Position fixed

We hebben geleerd dat layout elementen automatisch door de browser worden gepositioneerd, dit noemen we "document flow" of ["normal flow"](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow). Er zijn gevallen waarin je zelf de positie van een element wil hardcoderen, waarbij het geen deel uitmaakt van die flow. *Bijvoorbeeld: een chat venster dat altijd rechtsonderin je pagina blijft staan.*. Met de eigenschap `position:fixed` wordt een element uit de flow gehaald. Je kan het nu zelf positioneren met `bottom, top, left, right`. Het element blijft op die plek staan zelfs als het venster scrolled. 

```css
.chatwindow {
    position:fixed;
    bottom:20px;
    right:20px;
}
```
### Sticky

Een sticky element krijgt een `fixed` position zodra de gebruiker een bepaald punt voorbij scrolled. Dit werkt goed voor `nav` elementen. 

```css
nav.sticky {
  position: sticky;
  top: 20px;
}
```

<br><br><br>

## Klassikale oefening

### Transition op nav bar

- Plaats een `hover` effect op je nav bar buttons.
- Gebruik `transition` om de hover te animeren.

### Fixed nav bar

- Gebruik `position:fixed` en `top:0` om de nav bar vast te zetten, zelfs als de pagina scrolled.

### Fancy cards

- Plaats een aantal divs naast elkaar met de class `card`.
- On `hover` maak je de card groter met `transform:scale(1.1)` en je voegt een schaduw toe met `box-shadow`.
- Geef de card een `transition` zodat de animatie geleidelijk gaat.

### Chat request

- Ontwerp een chat window in een eigen div element, onder je andere html code.
- Gebruik `position fixed` met `bottom, right` om het chat window rechtsonderin beeld te fixeren, ongeacht de scroll positie.
- Met `transform:translateX()` plaats je nu het chat window rechts *buiten* beeld
- Ontwerp een `@keyframes` animatie die de `translateX()` weer terug op 0 zet.
- Gebruik `animation` om het chat window te animeren. De animatie speelt maar 1x, dit doe je met `forwards`.

<br><br><br>

## Zelfstandige oefening

Kies een van de oefeningen om mee aan de slag te gaan.

<br>

***Cards falling in place***

- Plaats een aantal `cards` naast elkaar met `flex`. Dit is de eindpositie.
- Ontwerp een startpositie, van waaruit de card in beeld gaat vallen. Dit doe je met `opacity` en verschillende `transforms`, zoals `scale`, `rotateY` en `translateZ`.
- Gebruik `keyframes` en `animation` om de cards naar de eindpositie te animeren. De animatie speelt maar 1x, dit doe je met `animation forwards`.
- Gebruik `animation-delay` om ***elke kaart*** een eigen delay te geven. Zo kan je de kaarten *na elkaar* in beeld laten vallen.
- Experimenteer met de verschillende `ease` opties. Wat doet dit precies? Je kan op [deze site](https://easings.net/#) verschillende `eases` uitproberen en copy>pasten.

***Audio bars***

- Plaats vijf divs naast elkaar in een flex container. Geef de divs een afmeting en achtergrondkleur.
- Je kan de achtergrondkleur van groen naar rood laten lopen met [CSS Gradient](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/linear-gradient)
- Gebruik `keyframes` om een animatie te ontwerpen, de bars kunnen groeien en krimpen.
- Gebruik `animation` om elke bar te laten bewegen. Door de `time` en `ease` per bar te veranderen bewegen alle bars verschillend.

<img src="https://github.com/HR-CMGT/frontend-2023-2024/assets/6097853/93c03d37-f405-40f8-a07e-3c5b7fdca1a9" width="100" />

<Br><br><br>
  
## Links
  
- [Animeer de header image kleuren](https://codepen.io/tommiehansen/pen/BaGyVVy)
- [W3Schools animations](https://www.w3schools.com/css/css3_animations.asp)
- [MDN Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)
- [Animeer een SVG illustratie](https://codepen.io/eerk/pen/ZPzNqv)
- [Custom easing](https://easings.net/)
- [CSS Filter](https://developer.mozilla.org/en-US/docs/Web/CSS/filter-function)
- [🤯 Backface Visibility](https://css-tricks.com/almanac/properties/b/backface-visibility/) en [voorbeeld](https://codepen.io/eerk/pen/WNLdrLK)

