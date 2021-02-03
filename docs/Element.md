# Element.io (tchat, alternative à Slack)
<div class='btn-vide'>

[<i class="fa fa-external-link" aria-hidden="true"></i> Application Element.io](https://app.element.io/)

</div>

## Introduction

`Element.io` est une application permettant de communiquer de façon efficace et sécurisé. Cette application est une alternative à Slack très complète. Dans une même interface on peut discuter avec plusieurs groupes, partager des documents, écrire sur des documents communs et utiliser également le logiciel Jitsi pour faire des appels en visioconférence.

Un des nombreux avantages de Element.io c'est qu'on peut l'utiliser directement dans un navigateur [web](https://app.element.io/) mais qu'il existe aussi des clients pour [Android](https://play.google.com/store/apps/details?id=im.vector.app), [Iphone](https://apps.apple.com/app/vector/id1083446067), [Mac OS](https://packages.riot.im/desktop/install/macos/Element.dmg), [Windows](https://packages.riot.im/desktop/install/win32/x64/Element%20Setup.exe), et bien sûr [Linux](https://element.io/get-started).

!> L'instance [BigBlueButton](/BBB.md) est à privilégier pour vos visioconférences longues. Pour des petits points, l'outil de visioconférence intégré à Element.io peut être utilisé.

## Premier pas avec Element

### S'inscrire 

Pour s'inscrire il faut se rendre sur l'[application web](https://app.element.io/) et de cliquer sur `Créer un compte`. Ensuite, il faut choisir un serveur, pour le moment nous allons utiliser le serveur **Matrix.org**. Peut être que plus tard nous migrerons vers notre propre serveur. Votre navigateur va sans doute vous demander un accès au stockage persistant des données. Il faut accepter pour qu'Element puisse stocker vos clés et messages sur votre ordinateur. Vous devait ensuite renseigner votre nom d'utilisateur, un mot de passe ainsi qu'un email. L'email n'est pas obligatoire mais fortement conseillé pour pouvoir redemander son mot de passe si besoin. Le nom d'utilisateur et l'email 
permettrons aux gens veulent communiquez avec vous de vous retrouver.

!> La prochaine étape est un peu délicate, concentrez-vous. Un des principaux avantages de Element est le chiffrement de bout en bout [<i class="fa fa-wikipedia-w" aria-hidden="true"></i>](https://fr.wikipedia.org/wiki/Chiffrement_de_bout_en_bout). Pour cela, chacun de nous a besoin de générer une clé de Sécurité (attention, c'est différent du mot de passe). 
Lors de votre première communication à l'application, Element permet de `générer une clé de sécurité`. Il faut que vous stockiez précieusement cette clé quelque part (par ex. avec un gestionnaire de mot de passe comme celui de [Firefox](https://www.mozilla.org/fr/firefox/lockwise/) ou [KeePassXC](https://keepassxc.org/)). Elle vous servira à retrouver l'historique de vos conversations si vous perdez vos comptes et à vous authentifier quand vous utiliserez un nouveau périphérique (c'est à dire un nouvel ordinateur ou smartphone).

<!--  !> Pour l'instant nous allons utiliser des salons non chiffrés. Le chiffrement des discussions rends assez complexes certaines fonctionnalités. Lors de la création d'un nouveau salon il faut bien coché que l'on souhaite un salon non chiffrés. Les salons de discussions deux-à-deux sont toujours chiffrés.-->

### Un petit tour de l'interface

![Interface de l'application Element.io](_media/element.webp)

À droite (rectangle jaune), les **communautés** sont représentées par des badges qui vous permettent de filtrer les salons que vous regardez. Dans la colonne suivante votre nom d'utilisateur (rectangle blanc) permet, en cliquant dessus, d'ouvrir des options (mode sombres, paramètres…). Au dessous une barre de recherche permet de filtrer les salons. En cliquant sur la boussole on peut rechercher un salon public ou une personne. 

Encore en dessous (rectangle violet), vos salons sont classés selon plusieurs critères:
- Vos salons `favoris`. Pour mettre un salon en favoris il faut survoler le salon, cliquer sur <i class="fa fa-ellipsis-h" aria-hidden="true"></i> puis sur `favoris`.
- Les discussions directes (deux à deux) sont classés dans la catégorie `personnes`.
- Ensuite viennent les salons non classés favoris ni priorité basse.
- Puis les salons `priorité basse`.
- Enfin une section historique contiendra les salons que vous avez quitté ou qui ont été supprimé.

La colonne centrale (rectangle vert) est l'emplacement du texte de discussion. En bas de cette colonne se trouve la zone de texte (rectangle bleu) pour écrire un nouveau message ou partager des documents. 

Enfin, en cliquant sur le symbole <i class="fa fa-info-circle" aria-hidden="true"></i> en haut à droite on ouvre les options du salon à droite (rectangle rose) qui permettent notamment de voir les personnes qui participent au salon, de retrouver les fichier partagés ou encore de 
modifier les paramètres du salon. 


#### Le concept des communautés
 
Le protocole Matrix qui est utilisé par l'application Element.io permet de communiquer avec de nombreuses personnes, que ce soit sur des sujets professionnels ou privés. Pour regrouper les salons selon des thématiques on peut utiliser des communautés. Une communauté sert donc à regrouper des utilisateurs (par ex. les membres du « cercle pédago » de Scholae) qui partagent des salons communs.

?> Les communautés à Scholae serait aux nombres de deux initialement : la **communauté générale** (lycéen + adulte) et la communauté du **cercle pédago**. 

#### Le concept des salons

Dans les logiciels de communication le concept de **salons** (= canaux sous Slack) est central. Un salon regroupe un ensemble d'utilisateurs autour d'une thématique. Dans le cadre de Scholae, nous proposons l'organisation en Salon décrite ci dessous


- **Communauté générale** :
  - `Discussion générale` ![i](/_media/bagde_rect_G.svg ':class=img-in-text')
  - Seconde
    - `Seconde` discussion générale ![i](/_media/bagde_rect_2nd.svg ':class=img-in-text')
    - `2nd-Matière 1` (par ex. «2nd-SNT») ![i](/_media/bagde_rect_SNT_2nd.svg ':class=img-in-text')
    - `2nd-Matière …` 
  - Première
    - `Première` discussion générale ![i](/_media/bagde_rect_1er.svg ':class=img-in-text')
    - `1-Matière 1` (par ex. «1-NSI») ![i](/_media/bagde_rect_NSI_1er.svg ':class=img-in-text')
    - `1-Matière …` 
  - Seconde
    - `Terminal` discussion générale ![i](/_media/bagde_rect_Ter.svg ':class=img-in-text')
    - `T-Matière 1` (par ex. «T-NSI») ![i](/_media/bagde_rect_NSI_Ter.svg ':class=img-in-text')
    - `T-Matière …` 

- **Cercle pédago** :
  - `Discussion générale` ![i](/_media/bagde_G.svg ':class=img-in-text')
  - `Calendrier`  ![i](/_media/bagde_cal.svg ':class=img-in-text')
  - `Vie de l'élève` ![i](/_media/bagde_vde.svg ':class=img-in-text')
  - `2nde` ![i](/_media/bagde_2nd.svg ':class=img-in-text')
  - `1ère` ![i](/_media/bagde_1er.svg ':class=img-in-text')
  - `Term` ![i](/_media/bagde_Ter.svg ':class=img-in-text')

#### Le concept des fils de discussion

Dans un salon, plusieurs discussions peuvent avoir lieu. Il est donc important de n'écrire un nouveau message que si le sujet est nouveau. Quand on veut réagir à un autre message il y répondre. Pour cela, en passant la souris sur le message on voit apparaître une liste de 3-4 boutons :
- Réagir (à l'aide d'un émoticône)
- Répondre
- Modifier le message (ce bouton n'apparaît que pour les messages dont on est l'auteur)
- Autres options


#### À qui je parle ? Qui à vu mes messages ?

Toutes les personnes qui sont inscrites dans le salon peuvent voir vos messages. La liste des personnes qui ont accès au salon se trouve dans la colonne de droite lorsque l'on clique sur l'icone  <i class="fa fa-info-circle" aria-hidden="true"></i>. 

À côté de chaque message, vous avez également une liste de badge qui indique qui a vu vos messages.

#### Comment j'écrit du texte ?

Vous pouvez utilisez le format [markdown](https://daringfireball.net/projects/markdown/) dans vos messages. C'est très simple, par ex. pour mettre un mot en gras on utilise entoure un mot avec deux étoiles. Pour indiquer un titre de rang 2 on utilise deux # devant le titre. Pour faire un lien hypertexte on met le texte du lien entre crochet puis l'adresse du lien entre parenthèse. Vous pouvez jouer avec ce langage sur le site [Dillinger](https://dillinger.io/).

Par ailleurs, quand vous tapez sur la touche `entrée`, vous envoyez le message. Pour passer à la ligne il faut tapez sur la touche `entrée` tout en maintenant la touche `maj` enfoncée.


## Les paramètres importants

### Les paramètres de notification

## Astuces

Pour partager son écran il faut cliquer sur la caméra en bas à gauche de la zone de texte tout en maintenant la touche `Maj` enfoncée.