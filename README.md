# sonde
sondeur ultrason immergeable pour plongeur
---
la fonctionnalité est d'utiliser le dispositif en plongée pour faciliter la localisation d'une épave lorsque la visibilité est réduite.
Après être arriver sur le fond, le plogeur ne voit pas l'épave car il est arrive à coté.
La sonde est a utiliser horizontalement en faisant un tour de 360 °.
La sonde émet une oonde ultrason et recoit un echo si l'obstacle est dans sa direction.
Cela donne une indication au plongeur pour se diriger vers l'echo, donc l'épave
Plus besoin d'utiliser un dévidoir et de prendre du temps de recherche et palmage au fond.
La détection ne doit pas etre au-dela de 30 à 40 m , car c'est une distance importante surtout si l'épave dépassse peu du relief du fond.
---
Le dispositif comprend:
  _ un transducteur ultrason à 40 kHz étanche
  - une carte JSN-SR04T-2.0
  - un ESP 32 Upsy Wroom ou equivalent avec chargeur de batterie LiPo
  - un ecran OLED SSD1306
  - un convertisseur DC/DC LiPo vers 5 v pour alimenter la carte JSN.
---
Le fonctionnement prévu est :
- l'ensemble est étanche et se raccorde à terre sur une embase USB 3.0 pour charge la batterie, voir modifier le code de l'ESP 32
- lil y a un bouchon amovible pour protéger le connecteur USB lors de l'immersion
- la mise en service se fait par des contacts humides lors de l'immerssion
- la mise à l'arrêt se fait par une temporisation après retour au sec des contacts humides
- l'affichage annonce à la mise en service un OK avec le niveau de charge de la batterie, puis bascule en mode actif
- l'affichage du mode actif est un rafraichissement toutes les secondes de la mesure , mesure en mètre et décimètre
