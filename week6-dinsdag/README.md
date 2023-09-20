# Week 6 - Dinsdag

- UI design
- Transform, 3D, filter
- Transition
- Animation
- Position absolute, fixed

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


<br><br><br>

## Oefening

Chat request popup

- `position absolute` haalt een element uit de document flow. Dit werkt goed voor popups, chat venster, overlay.
- `left, top, bottom, right` bepaalt de basis positie
- `transform` gebruik je als je een item wil animeren
- `transition` is animatie die afspeelt na een gebruikers interactie (zoals `hover` of `scroll`)
- `animation` is animatie die automatisch kan afspelen

<Br><br><br>
  
## Voorbeelden
  
- [Animeer de header image kleuren](https://codepen.io/tommiehansen/pen/BaGyVVy)
- [CSS Filter](https://developer.mozilla.org/en-US/docs/Web/CSS/filter-function)
