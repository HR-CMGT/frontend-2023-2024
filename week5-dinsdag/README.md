# Week 5 - Dinsdag

> *“A Pixel is Not a Pixel”*

- [Week 5 - Dinsdag](#week-5---dinsdag)
  - [Responsive design](#responsive-design)
  - [Afbeeldingen](#afbeeldingen)
  - [Relatieve units](#relatieve-units)
  - [Links](#links)

<br><br><br>

## Responsive design

- meta-viewport
- Werken met `vw` `vh`, `%`, `em` en `rem`.
- Media queries
- Flex row naar flex column

<br><br><br>

## Afbeeldingen

- Door alleen de hoogte of breedte aan te passen blijft de verhouding correct
- Images plaats je meestal in een container. De image afmeting is 100% van de container. De maat van de container bepaal je met flex.
- Aspect-ratio
- Afbeeldingen in je images folder hebben vaak niet dezelfde verhouding. 
- Werken met object-fit
- Werken met achtergrond afbeeldingen
- Werken met DPI waarden: `srcset`
- Werken met `picture`
- Lazy loading

<br><hr><br>

## Absolute en relatieve units

| Eenheid | Voorbeeld       | Toepassing                                   |
|---------|-----------------|----------------------------------------------|
| px      | width:100px;    | Een absolute pixel afmeting                  |
| vw      | width:40vw;     | 40vw betekent 40% van de viewport width      |
| vh      | height:30vh;    | vh betekent % van de viewport height         |
| %       | width:20%;      | De breedte is 20% van de parent container    |
| %       | font-size:120%; | De font size is 120% van de parent font-size |
| rem     | font-size:2rem; | De font size is 2 maal de default font size  |




<br><br><br>
 
## Links
  
- [Guide to responsive images](https://elad.medium.com/a-complete-guide-for-responsive-images-b13db359c6c7)
- [Werken met `srcset` en `picture`](https://css-tricks.com/a-guide-to-the-responsive-images-syntax-in-html/)
- [Lazy Loading](https://www.w3schools.com/tags/att_img_loading.asp)
- [Youtube responsive images](https://www.youtube.com/watch?v=fp9eVtkQ4EA)
- [CSS Units](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units)
