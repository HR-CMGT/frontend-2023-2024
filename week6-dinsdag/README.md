# Week 6 - Dinsdag

- UI design
- Transform, 3D, filter
- Transition
- Animation
- Position fixed
- Oefening

<br><br><br>

## UI design

- Voor wie is jouw website bedoeld?  Wat is het doel van de website? Kies een uitstraling die hier bij past.
- Kies een *kleurpalet*, bv. door kleuren uit je header foto te halen, of via een tool : [Coolors](https://coolors.co), [Adobe](https://color.adobe.com/create/color-wheel), [Colormind](http://colormind.io) 
- Gebruik [Google Fonts](https://fonts.google.com) om twee lettertypes te kiezen: een fancy lettertype voor je kopteksten, en een prettig leesbaar lettertype voor je body tekst.


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
> 🤯 Gebruik de [Backface Visibility](https://css-tricks.com/almanac/properties/b/backface-visibility/) optie om andere content op de achterkant van een div te laten zien!

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

## Oefening

***Chat request popup***

- `position fixed` met `left, top, bottom, right` plaatst een chat window rechtsonder in beeld
- met `animation` en `transform` laten we het chat window van rechts buiten beeld, naar binnen animeren.
- we maken een aparte animation om aandacht te vragen, bv. door de achtergrondkleur te laten oplichten

***Spinning card met achterkant***

- Gebruik `hover` om een `card div` 180 graden te roteren op de Y as
- Gebruik `perspective` om een diepte effect te krijgen
- Gebruik d[Backface Visibility](https://css-tricks.com/almanac/properties/b/backface-visibility/) om andere content op de achterkant te laten zien

<Br><br><br>
  
## Links
  
- [Animeer de header image kleuren](https://codepen.io/tommiehansen/pen/BaGyVVy)
- [W3Schools animations](https://www.w3schools.com/css/css3_animations.asp)
- [MDN Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)
- [CSS Filter](https://developer.mozilla.org/en-US/docs/Web/CSS/filter-function)
