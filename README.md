Lafint
======
Template de clavier qwerty international basé sur le clavier qwerty-lafayette.

basé sur <https://qwerty-lafayette.org/>

Disclaimer
----------
Ce projet contient uniquement la customization au format toml du clavier. 
Toute la complexité est donc portée par les créateurs du projet Qwerty-Lafayette, dont je ne fais pas partie.

QuickStart
===========

Installation Linux
------------------

    sudo cp lafint.xkb_symbols /usr/share/xkeyboard-config-2/symbols/lafint
    setxkbmap lafint

Installation Windows
--------------------

Build et modifications
---------------------
Partir d'une des 2 sources [lafint.toml](lafint.toml) ou [lafint1.toml](lafint1.toml).
Construire avec [Kalamine](https://github.com/OneDeadKey/kalamine)
 - kalamine build lafint.toml
Installer ou tester avec [XKalamine](https://github.com/OneDeadKey/kalamine)
 - xkalamine apply lafint.toml


Utilisation
-----------
![layout](dist/lafint.svg)

Tous les clavier qwerty internationaux lafayete et lafint se basent sur une touche morte, que l'on presse pour faire un accent avant de presser la voyelle.
Cette touche morte est notée "🟉" dans la disposition ci-dessus, elle est à la place de la touche ⌨️; sur le lafayette, et de ⌨️' en lafint et en international

Voila les différences essentielles du lafint par rapport à un qwerty international: 
 - la touche d'accent ' ou 🟉 est plus orientée français et va doc produire les accents utilisés en français ,"éèê" etc., et aussi la cédille, le oe lié.
 - la touche ; est réutilisée pour produire une single quote ' en accès direct. ce caractère est beaucoup trop utilisé en français pour être en accès indirect
 - le caractère ; est produit par la combinaison 🟉; . on a réutilisé cette touche, mais les 2 touches sont côte à côte, c'est assez facile de mémoriser le pattern.

Voila les différences essentielles du lafint par rapport à un qwerty lafayette:
 - remettre la touche morte sur la meme touche qu'en qwerty international pour faciliter la mémorisation des touches
 - remettre les caractères <> en accès shift ( il faut utiliser altgr avec le lafayette)
 - globalement on peut se servir de ce clavier sans utiliser le altgr
 - le ; qu'on a perdu en accès direct pour cause de réutilisation de touche se fait maintenant en accès indirect
 - les disposition de l'accents é, se fait comme en qwerty international plutot qu'en lafayette ( pas très clair mais à l'utilisation vous comprendrez)
 - Sur le shift touche morte 🟉, la touche redevient un accès direct pour conserver la touche " d'origine du qwerty international.
 



Explications
============

Pourquoi le qwerty?
-------------------
En 2 phrases: tous les langages de programmation, y compris la ligne de commande, sont optimisés en qwerty, les symboles utilisés sont tous regroupés, logique et disponible en accès direct.
je citerais par exemple les caractères {}[]|\'"<> tous sur la meme colonne de droite. 
Et enfin les nombre en accès direct ça change tout au quotidien sur un clavier petit format, sur portable etc.

Et pour les français ce clavier ne pose pas de problème, je peux utiliser tous les accents de l'azerty + les accents majuscules non possibles en azerty.
Les dispositions utilisables pour le français sont pour moi:
 - le qwerty international, disponible de partout
 - le qwerty lafayette, facile à installer depuis le site dédié
 - le qwerty lafint (Lafayette International) intermédiaire entre les 2
 
 
Pourquoi mon propre format
--------------------------
Honnêtement, le Qwerty-Lafayette est plus abouti. Si vous tombez ici par hasard, essayez d'abord le Qwerty-Lafayette pour comparer. 
Voici pourquoi j'ai fait une autre disposition :
 - Pour utiliser Kalamine, l´outil qui sert a génerer aussi lafayette. c'est un outil de customisation amusant
 - Pour switcher plus facilement entre qwerty us international  et personnalisé (lafayete ou lafint)
 - Parce que le qwerty international est un peu plus lourd a utiliser (ê se tape en 2 touches shift ^ puis e, l'accet grave est loin des touches classiques, et l'apostrophe en accès indirect)
 - Parce que le qwerty lafayette nécessite de réapprendre un peu plus le clavier.
 - Parce que je regarde mon clavier quand le tape, meme si c'est mal, et en qwerty international ou lafint, les touches correspondent bien a un qwerty us. 
 

Alternative le lafint 1ère version
----------------------------------
J'ai conservé les 2 dispositions lafint1 et lafint tout court en version 2. l'intérêt du lafint1 est qu'il est beaucoup plus proche du qwerty international, 
mais avec l'iconvénient dávoir lápostrophe en accès indirect, ce qui provoque pas mal de fautes comme on le voit sur cette phrase.

A vous de voir si vous préférer galérer avec les apostrophes ou avec les point virgules: c'est quoi que vous utilisez plus: ' ou ;?

