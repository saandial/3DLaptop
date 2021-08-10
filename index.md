---
layout: default
---

L'autonomie en vol d'un drone peut varier en fonction de plusieurs critères comme son poids, sa taille, les hélices, la batterie, les rmoteurs, la consommation des composants électroniques etc. 

Bref autant de critères qui selon la conception peuvent influer sur l'autonomie de la batterie et par conséquence sur le temps de vol. Je réalise ici quelques tests de configurations d'un drone de type quadcopter entièrement imprimé en 3D afin d'optimiser le temps de vol. 

Pour cela nous allons faire varier principalement les trois critères suivants : la batterie, les moteurs et les hélices, bien évidemment le poids du drone sera aussi variable selon les choix des conceptions. Commençons par analyser les caractéristiques physiques et techniques du drone.

# Dimensions et poids du châssis à vide :

![Front](./local/images/front.png)

# Caractéristiques techniques :

Pour réaliser ces tests ce drone sera équipé d'un contrôleur de vol BeagleBone Blue. BeagleBone Blue est un mini ordinateur monocarte Open Source sous Linux spécialement conçu pour des applications embarquées. Il est équipé des systèmes de communication sans fil standard Wi-Fi et Bluetooth 4.0 ainsi que des connecteurs dédiés pour d'autres interfaces telles que UART, SPI, radio DSM2, et GPS. Il embarque également une unité de mesure inertielle indispensable pour l'orientation d'un drone comportant un accéléromètre, un gyroscope et une boussole. Voici la liste des composants électroniques embarqués dans le drone :

*   Contrôleur de vol
*   Moteur Brushless x 4
*   ESC x 4
*   Batterie LiPo 11.1 V
*   Ubec 5V3A
*   Module GPS
*   Recepteur radio
*   Radio 3DR
*   Raspberry Pi Zero W couplé en liaison série à un microcontrôleur Atmega328(*)

(*) Le Raspberry Pi Zero W couplé en liaison série à un microcontrôleur Atmega328 mesure l'état actuel de la batterie tout au long du test. Les mesures stocké dans un fichier sont ensuite transmis à la station de contrôle au sol.

# Stratégie de test :


type de vol etc. sa dimension Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
