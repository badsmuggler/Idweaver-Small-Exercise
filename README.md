# Exercice Frontend (Temps estimé 4h)

## Design

Vous pourrez trouver les différents fichiers ".psd" dans le dossier "Design", à savoir les version desktop et mobile de l'exercice ainsi que les polices de caractère à utiliser. Voici également le lien vers la police "google font": https://fonts.google.com/?query=roboto&selection.family=Roboto

## Développement

Dans le dossier "Development", vous trouverez un boilerplate de travail qu'il vous est libre d'utiliser (ou pas). Les points qui seront évalués sont les suivants:

 * HTML5 et CSS3
 * Javascript Native
 * L'organisation / méthodologie
 * La maintenabilité et la réutilisation du code

L'utilisation d'un framework JS tel que VueJS ou React est autorisée mais pas obligatoire. Par contre, l'utilsation de jQuery et/ou de plugins divers est interdite. On privilégiera le développement en javascript natif ES6 et +.

### Ce qui est attendu

 * La mise en place d'une configuration gulp ou webpack.
 * L'intégration responsive, adaptative, précise et rigoureuse (HTML5, CSS3) des designs fournis.
 * Le développement javascript pour la validation d'un numéro de carte de crédit (voir explication ci après).

### La validation de la carte de crédit

La validation se fera exclusivement au "keyup" et devra fournir les informations suivantes :

 * Le type de la carte de crédit (Visa, Mastercard, Amex)
 * Le fond blanc derrière le type de la carte deviendra vert (success), rouge (error) ou orange (si le type de la carte n'est pas connu).

Quelques informations sur la validation des cartes de crédit :

 * Les cartes *Visa* commencent par un `4`. Elles ne sont valides que si elles comptent entre `13` et `16` chiffres.
 * Les cartes *Mastercard* commencent avec un `5`. Elles ne sont valides que si elles comptent `16` chiffres.
 * Les cartes *American Express* commencent avec un `3`. Le second chiffre sera un `4` ou un `7`. Elles ne sont valides que si elles comptent `15` chiffres.

En bonus, il existe un algorithme qui permet de controler la validité des numéros de carte de crédit. Il vous faudra le trouver et l'implémenter dans votre solution (par exemple en coloriant le fond en mauve).
