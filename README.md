# Formation front end 2

#### Sujets abordés

##### Pseudo elements
https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements

##### CSS Transitions
https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions

##### CSS Transforms
https://developer.mozilla.org/en-US/docs/Web/CSS/transform

##### Custom properties (--*)
https://developer.mozilla.org/en-US/docs/Web/CSS/--*

##### CSS Animations
https://developer.mozilla.org/en-US/docs/Web/CSS/animation


## Exercices
Inspiration : https://dribbble.com/shots/5682803-February

Chaque exercice est basé sur une des différentes branche de ce repo. Le premier exercice commence sur la branche 1.0 et l'exercice 2 sur la branche 2.0.

Chaque branche contient la solution de l'exercice précédent.

### Exercice 1
Le but de cet exercice est de se familiariser avec les pseudo elements. Pour ce faire, vous devez :

1- Ajouter une pastille rouge (#E7040F) autour du jour courrant (.date-current).

2- Ajouter les points rouges (#E7040F) en dessous des dates contenant des notifications (.date-notif).

3- Ajouter les points noirs (#001B44) en dessous des dates flaggées comme "busy" (.data-busy).

### Exercice 1.5
Le but de cet exercice est de se familiariser avec les transitions CSS. Pour ce faire, vous devez :

1- Sur hover des dates du mois courant ajouter un cercle rouge (#E7040F) derrière la date, et afficher le texte en blanc.

2- Assurez-vous que la transition n'est par 0 - 1 mais smooth.

3- Le texte devrait changer de couleur plus rapidement que le fond.

### Exercice 2
Le but de cet exercice est de sa familiariser avec les CSS Transforms. Pour ce faire, vous devez:

1- Centrer le contenu de la pastille du jour courant en utilisant la proprités transform. 
2- Donner un angle de 5 deg et un scale de 1.2 au TUESDAY, au hover donner un scale de 1

### Exercice 3
Le but de cet exercice est de se familiariser avec les variables CSS. Pour ce faire, vous devez checkout la branche `3.0` et ensuite :

1- Ajouter le snippet suivant entre les lignes 66/67 du fichier `html.html`:

```
<div class="mt6">
    <div class="picker flex mb2">
        <input type="text" placeholder="#hex" class="br2 h2 ba b--gray color-picker-input pa2 mr2">
        <button class="br2 bn h2 bg-light-red white color-picker">Set primary color</button>
    </div>
    <div class="picker flex">
        <input type="text" placeholder="#hex" class="br2 h2 ba b--gray paper-color-picker-input pa2 mr2">
        <button class="br2 bn h2 bg-light-red white paper-color-picker">Set paper color</button>
    </div>
</div>
<script>
    const calendar = document.querySelector(".calendar");
    const colorPicker = document.querySelector(".color-picker");
    const paperColorPicker = document.querySelector(".paper-color-picker");
    const root = document.documentElement;

    /* add listener on the click event of the colorPicker and change the primary color */

    /* add listener on the click event of the paperColorPicker and change the paper color */

</script>
```

2- À l'aide de variables CSS, modifier les deux couleurs dans les différents event listener. 

Pratiquez vous avec les CSS properties afin de réutiliser certaines valeurs qui sont utilisées à plusieurs reprises

### Exercice 4
Lorsque l'on hover sur une date clé (avec un point dessous) animez le point

Bonus : animer le calendrier lorsqu'on clique dessus pour qu'il disparaisse de manière "naturelle".

### Exercice 5
Ajouter une tempête de neige à la partie gauche du calendrier.

Conseil: Utilisez la propriété "background-image" combiné avec une animation par @keyframe

Snow1 https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-large-075d267ecbc42e3564c8ed43516dd557.png
Snow2 https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-medium-0b8a5e0732315b68e1f54185be7a1ad9.png 

Mettre ce snippet 
après la classe calendar-illu.png
```
<div class="calendar-illustration__item">
    <img src="calendar-illu.png" alt="Snow">
    <div id="snow-front" class="absolute z2 w-100 h-100 "></div>
    <div id="snow-deep" class="absolute z2 w-100 h-100 "></div>
</div>
```
