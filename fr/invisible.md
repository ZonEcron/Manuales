# ZonEcrón© Invisible  
## Manuel d'Utilisateur  

![Saut](../images/invisible/hurdle.png)  

## Contenu  

1. [Introduction](#1-introduction)  
   - [1.1 Objectif de l'appareil](#11-objectif-de-lappareil)  
   - [1.2 Caractéristiques principales](#12-caractéristiques-principales)  
   - [1.3 Comparez-nous](#13-comparez-nous)  
2. [Utilisation](#2-utilisation)  
   - [2.1 Montage et mise en marche](#21-montage-et-mise-en-marche)  
   - [2.2 Alignement et détection](#22-alignement-et-détection)  
   - [2.3 Auto-interférences infrarouges](#23-auto-interférences-infrarouges)  
   - [2.4 Communication radio](#24-communication-radio)  
   - [2.5 Visualisation sur écran](#25-visualisation-sur-écran)  
   - [2.6 Alimentation et recharge](#26-alimentation-et-recharge)  
   - [2.7 Autonomie](#27-autonomie)  
   - [2.8 Soleil et pluie](#28-soleil-et-pluie)  
   - [2.9 Stockage](#29-stockage)  
3. [Épilogue](#3-épilogue)  
4. [Contact](#4-contact)  

---

## 1 Introduction  

### 1.1 Objectif de l'appareil  

Le ZonEcrón® Invisible—et quand nous disons ZonEcrón®, imaginez des lumières néon et des feux d'artifice, etc.—a été conçu comme un remplacement des systèmes conventionnels qui sont généralement installés à côté ou au-dessus du premier et du dernier saut, et qui, dans une certaine mesure, gênent la course du guide ou du chien.  

Avec cet objectif en tête et notre inclination naturelle à minimiser les efforts, nous avons ajouté une série de conditions similaires à celles du ZonEcrón® original : installation facile, pas de câbles, etc. En nous appuyant sur notre expérience dans le développement du ZonEcrón® original, nous avons également inclus des exigences comme le maintien d'une hauteur de détection constante et l'installation de tous les éléments à l'intérieur des ailes d'un saut.  

Ainsi, le ZonEcrón® Invisible (désormais simplement ZonEcrón®) a été créé dans le but d'améliorer les systèmes de chronométrage actuellement disponibles, offrant une plus grande simplicité d'utilisation et une sécurité accrue pour les chiens et leurs guides.  

---

### 1.2 Caractéristiques principales  

- Invisible (ou presque) : tous les composants sont intégrés dans la structure des ailes.  
- Rapide à installer : aussi rapide que de monter un saut.  
- Adapté à l'extérieur : résistant au soleil et à la pluie.  
- Rechargeable : via USB, avec une autonomie supérieure à 30 heures.  
- Sécurisé : signaux inoffensifs (infrarouges et Wi-Fi) et aucune arête vive.  
- Sans fil : aucun câble utilisé, sauf pour recharger les batteries.  
- Portée de communication étendue : testé jusqu'à 200 m, recommandé à 40 m.  
- 6 capteurs : plus besoin de déplacer les cellules lors des changements de hauteur.  

---

### 1.3 Comparez-nous  

Nous pensons avoir développé un produit unique en termes de fonctionnalités. Nous n'avons trouvé aucun autre produit réunissant toutes les caractéristiques du ZonEcrón®, que nous ne répéterons pas ici.  

Lorsque nous avons ressenti le besoin d'un chronomètre de compétition, nous avons cherché longtemps et sérieusement. Nous avons trouvé d'autres produits avec le même objectif, mais aucun ne répondait à toutes nos exigences, ce qui nous a poussés à créer le nôtre.  

Si vous avez des besoins spécifiques que le ZonEcrón® ne satisfait pas, il existe d'autres produits similaires. Nous vous invitons à chercher, comparer, et si vous trouvez… eh bien, une pensée curieuse est une pensée éveillée.  

---

## 2 Utilisation

### 2.1 Montage et mise en marche

Le ZonEcrón® est installé dans la structure d’un obstacle, et comme il est invisible… nous l’avons appelé invisible… je vais devoir parler à l’équipe marketing parce qu’il ne semble pas qu’ils fassent beaucoup d’efforts. Pour chaque obstacle, une aile contiendra les émetteurs infrarouges (le capuchon supérieur a 1 LED et les finitions décoratives sont blanches), tandis que l’autre aile contiendra les récepteurs infrarouges (le capuchon supérieur a 2 LED et les finitions décoratives sont noires) :

|                   Émetteur                   |                    Récepteur                   |
|----------------------------------------------|------------------------------------------------|
| ![Émetteur](../images/invisible/emitter.png) | ![Récepteur](../images/invisible/receiver.png) |

Il est donc en réalité « presque invisible, » mais faites attention à ne pas placer deux ailes avec des émetteurs sur le même obstacle, car cela ne fonctionnera évidemment pas (ce ne serait pas la première fois que cela se produit). Les plus attentifs auront également remarqué que deux ailes avec des récepteurs sur le même obstacle ne fonctionneront pas non plus.

Avons-nous été suffisamment clairs ? Par précaution, chaque obstacle doit comporter une aile avec des émetteurs et une aile avec des récepteurs.

Une fois les ailes placées l’une en face de l’autre, il suffit de les allumer. L’interrupteur et le connecteur pour recharger la batterie se trouvent sous l’aile, à l’intérieur du profil horizontal. Ils sont protégés par un couvercle coulissant avec ressort. Faites glisser le couvercle et placez l’interrupteur en position allumée (I).

![Batterie](../images/invisible/battery.png)

Les LED (1 ou 2 selon le type) s’allument immédiatement. Dans le cas des récepteurs, elles restent allumées pendant 5 secondes le temps que la communication radio soit établie. Les LED bleues restent allumées pour indiquer que le ZonEcrón® est… voyons qui va le dire… très bien ! Elles restent allumées pour indiquer que le ZonEcrón® est en marche. Je vais également devoir parler à l’équipe R&D, car ils semblent suivre la voie du marketing.

---

### 2.2 Alignement et détection

Une fois l’émetteur et le récepteur placés l’un en face de l’autre et allumés, six faisceaux infrarouges sont créés entre les six émetteurs et les six récepteurs, permettant de détecter le passage de tout chien, quelle que soit sa hauteur :

![Faisceaux](../images/invisible/beams.png)

La LED blanche sur l’aile des récepteurs s’éteint si l’alignement est correct et s’allume pour indiquer qu’un des faisceaux a été interrompu. La LED reste allumée pendant au moins 0,5 seconde, ou si l’interruption dure plus longtemps, elle reste allumée aussi longtemps que l’interruption persiste.

Si une des barrières est interrompue, le chronomètre démarre ou s’arrête. Si, en raison de la position de la barre, une paire émetteur-récepteur reste bloquée en permanence, cette paire sera ignorée après 5 secondes, et la LED blanche s’éteindra. Plusieurs paires peuvent être bloquées simultanément si nécessaire, par exemple en ajoutant des barres sous celle de l’obstacle pour empêcher un chien de passer sous un saut lors d’un entraînement. La seule paire qui ne peut pas être bloquée de façon permanente est la supérieure.

![Faisceau bloqué](../images/invisible/beamsPole.png)

L’utilisation standard est pour un obstacle, mais elle peut également être utilisée pour chronométrer des séquences en positionnant les ailes sans barre, par exemple à la sortie d’un tunnel. Faites attention à ne pas placer l’émetteur et le récepteur trop près l’un de l’autre ou parallèlement à des murs, car la puissance de l’émetteur est suffisante pour rebondir sur des objets proches ou son éclat (invisible) peut contourner une main si les deux sont trop proches. Nous recommandons une distance minimale de 1 mètre. La distance maximale dépend de la quantité de lumière ambiante, variant de 2 mètres en plein jour à 20 mètres dans l’obscurité avec un éclairage artificiel.

---

### 2.3 Auto-interférences infrarouges

En raison de la puissance des faisceaux infrarouges, conçus pour fonctionner en plein soleil, il peut arriver qu’un récepteur capte des signaux provenant de deux émetteurs. Cet effet est plus prononcé en faible luminosité ou dans des espaces clos.

Le symptôme le plus évident est que la LED blanche d’un récepteur s’allume et s’éteint constamment, et que le chronomètre peut démarrer et s’arrêter sans qu’aucun faisceau ne soit interrompu.

Cela peut se produire si les ailes ne sont pas bien alignées. Par exemple :

![Auto-interférences](../images/invisible/selfInterference.png)

Dans ce cas, le récepteur 1 (R1) reçoit les signaux de l’émetteur 1 (E1) et de l’émetteur 2 (E2), ce qui provoque une confusion.

Pour éviter cela, placez les deux récepteurs dans des directions opposées, de sorte qu’ils ne puissent recevoir les signaux que d’un seul émetteur. Dans l’exemple précédent, procédez ainsi :

![Pas d’auto-interférences](../images/invisible/noSelfInterference.png)

---

### 2.4 Communication radio

La communication radio s’établit automatiquement entre les cellules et d’autres accessoires possibles de la famille ZonEcrón®. Cette communication utilise la plage de fréquences Wi-Fi et peut être affectée dans des environnements où de nombreux réseaux Wi-Fi sont actifs.

Chaque récepteur contient une antenne interne pour établir cette communication. La portée maximale théorique est de 80 mètres en terrain dégagé. Nous avons testé une portée de 200 mètres dans un parc résidentiel avec plusieurs réseaux Wi-Fi environnants, sans problèmes de communication. Pour une performance optimale, nous recommandons de ne pas dépasser 40 mètres dans une piste de dimensions réglementaires.

---

### 2.5 Visualisation sur écran

Contrairement au ZonEcrón® original, le système invisible ne dispose pas d’un écran intégré. Pour visualiser les temps, un panneau d’affichage ZonEcrón® ou un dongle ZonEcrón® connecté à un ordinateur avec notre application sera nécessaire. Veuillez consulter les manuels de ces éléments pour plus d’informations.

---

### 2.6 Alimentation et recharge

Les quatre appareils (deux émetteurs et deux récepteurs) sont équipés d’une batterie interne au lithium rechargeable, ce qui élimine le besoin de câbles d’alimentation ou de communication pendant leur utilisation.

Les niveaux de batterie peuvent être consultés via l’application ZonEcron ou sur l’écran ZonEcron, selon le système d’affichage utilisé. Nous vous recommandons de consulter les manuels spécifiques pour plus de détails. De plus, les appareils indiquent le niveau de batterie grâce au clignotement des LEDs bleues :
- **Batterie supérieure à 30 %** : LED bleue fixe.
- **Batterie entre 30 % et 15 %** : clignotement lent de la LED bleue.
- **Batterie inférieure à 15 %** : clignotement rapide de la LED bleue.

Cet indicateur de charge est **approximatif**, car il est basé sur la mesure de la tension de la batterie, qui ne reflète pas toujours précisément la charge restante. Par conséquent, il est normal que la charge diminue rapidement de 100 % à 90 %, reste stable entre 90 % et 10 %, puis chute rapidement de 10 % à 0 %. Nous recommandons de ne pas trop décharger la batterie pour éviter des surprises désagréables du genre "oh non".

Les appareils disposent d’un port USB-C situé en bas, à côté de l’interrupteur. Pour recharger les batteries, les appareils doivent être éteints, et il suffit de connecter un câble USB standard à un chargeur USB. Grâce à la conception des connecteurs USB, il n’est pas physiquement possible de les brancher de manière incorrecte, ce qui garantit la sécurité même pour les utilisateurs les plus maladroits.

**ATTENTION : TEMPÉRATURES EXTRÊMES.**

Les batteries au lithium fonctionnent dans une plage de températures de 5 °C à 50 °C. En dehors de cette plage, la puissance fournie peut fluctuer, entraînant un comportement erratique du chronomètre. De plus, l’autonomie sera réduite.

Nous déconseillons fortement l’utilisation ou la recharge des batteries en dehors de cette plage, surtout lorsqu’elles sont trop froides, car cela pourrait considérablement réduire leur durée de vie ou les rendre inutilisables. Si la journée a été particulièrement froide ou chaude, éteignez les appareils et laissez-les dans un environnement tempéré. Attendez une heure pour qu’ils s’ajustent avant de les recharger.

**ATTENTION : NE PAS RECHARGER LES APPAREILS SANS SURVEILLANCE.**

Aucun appareil à batterie ne doit être rechargé sans surveillance. Il est courant de laisser son téléphone charger toute la nuit sans problème, mais cela ne signifie pas que des incidents ne peuvent pas se produire. Récemment, une grande entreprise a rencontré des problèmes avec les batteries de ses téléphones, qui surchauffaient lors de la charge et explosaient. Par conséquent, protégez-vous et protégez vos proches. Pas besoin de surveiller constamment pendant 4 heures, mais il est recommandé de rester à proximité lors de la recharge. Si cela n’est pas possible, débranchez-les et poursuivez la recharge ultérieurement. Ces batteries n’ont pas d’effet mémoire et peuvent être rechargées par intervalles sans problème.

**ATTENTION : INSPECTION EN CAS D’IMPACT.**

Il est probable qu’un chien percute l’aile où se trouve le ZonEcron© à un moment donné. Le design a été conçu pour rendre l’appareil aussi résistant que possible et pour fixer solidement les composants internes. Cependant, en cas d’impact, une inspection minutieuse est obligatoire. Si vous remarquez un dommage, si des pièces semblent bouger à l’intérieur ou si l’appareil surchauffe lors de la recharge, éteignez-le immédiatement, débranchez-le et placez-le dans un endroit sûr, loin des matériaux inflammables. Contactez-nous pour discuter des solutions possibles.

Le ZonEcron© dispose d’un circuit électronique qui contrôle la charge et la décharge des batteries. Il empêche les batteries d’être surchargées ou déchargées excessivement. L’indicateur de 0 % correspond au niveau minimum recommandé, à partir duquel le ZonEcron© doit être rechargé. Cependant, l’appareil restera allumé, exploitant la batterie au maximum, jusqu’à ce que le circuit de protection coupe l’alimentation. Cela peut être utile en cas d’urgence, mais ne doit pas devenir une habitude, car cela affecterait négativement la durée de vie des batteries.

Enfin, le conseil populaire selon lequel il faut décharger complètement une batterie avant de la recharger s’applique aux anciennes batteries au Ni-Cd. Pour ces batteries au lithium "modernes" (qui ne sont plus si nouvelles), **il est préférable de ne pas les décharger complètement** (en fait, cela est nuisible). Il est beaucoup plus conseillé de les recharger lorsqu’elles sont à mi-charge. Même les recharger par intervalles n’a aucun impact négatif.

---

### 2.7 Autonomie

Un appareil neuf a une autonomie de plus de 35 heures, ce qui est largement suffisant pour une compétition de deux jours. Cette autonomie diminuera avec le temps en raison du cycle de vie normal des batteries au lithium.

La température ambiante peut également affecter négativement la durée de vie de la batterie :
- Pendant l’utilisation : Plus il fait froid, moins la batterie durera. Il n’est pas recommandé d’utiliser les appareils à des températures inférieures à 0 °C.
- Pendant la recharge : Il est conseillé d’effectuer la recharge à des températures modérées, entre 10 °C et 30 °C, pour garantir une recharge correcte et complète.

Pour augmenter l’autonomie, les stratégies suivantes ont été adoptées :
- Lorsque le chronomètre fonctionne, la luminosité de l’écran est réduite, car l’information essentielle est le temps mesuré. Lorsque le chronomètre s’arrête, la luminosité de l’écran est augmentée.
- Après l’arrêt du chronomètre, au bout de 30 secondes d’inactivité, la luminosité de l’écran est encore réduite, et après 30 secondes supplémentaires, l’écran s’éteint, ne s’allumant que 1 seconde toutes les 5 secondes.

---

### 2.8 Soleil et pluie

Le ZonEcron original a été conçu pour fonctionner parfaitement en extérieur, sous le soleil ou la pluie.
- Sa couleur blanche caractéristique a été choisie spécifiquement pour éviter qu’il ne surchauffe au soleil.
- Son design permet une utilisation sous la pluie, à condition qu’il soit maintenu en position verticale avec les connecteurs orientés vers le bas, pour éviter l’entrée d’eau par les ouvertures.

---

### 2.9 Stockage

Lors du stockage du ZonEcron, il est important de prendre en compte l’humidité et l’état de la batterie :
- Comme mentionné précédemment, le ZonEcron **est résistant à la pluie, mais pas à l’humidité**. S’il reste humide plusieurs jours, l’humidité pénétrera progressivement dans le boîtier, ce qui peut endommager irréversiblement les composants électroniques. Par conséquent, s’il a été utilisé sous la pluie, laissez-le dans un environnement sec pendant une journée avant de le ranger pour éliminer toute humidité résiduelle.
- En ce qui concerne la batterie : Si vous prévoyez de ne pas utiliser le ZonEcron© pendant une longue période, **il est préférable de laisser les batteries à moitié chargées** pour maximiser leur durée de vie. Stocker des batteries au lithium complètement chargées ou déchargées pendant de longues périodes peut considérablement réduire leurs performances.

---

### 3 Épilogue

Profitez de votre temps avec vos chiens, et ne vous laissez pas frustrer en comparant vos temps avec ceux des autres (même si une saine compétition rend les choses plus amusantes). Vous ne devez rivaliser qu’avec vous-même.

Ce chronomètre est conçu pour rendre vos compétitions plus simples, tant pour l’utilisation que pour les changements de hauteur.

Nous espérons que vous tirerez le meilleur parti du ZonEcron©, et rappelez-vous : Pas d’erreurs par paresse… Donnez tout, allez !

---

### 4 Contact

Pour toute assistance technique, question ou suggestion, vous pouvez nous contacter par e-mail : [zonecron@gmail.com](mailto:zonecron@gmail.com)
