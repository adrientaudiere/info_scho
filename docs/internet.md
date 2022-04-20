# Internet à Scholae

## Le serveur proxy

Il s'agit d'un petit boîtier qui réglemente l'accès à Internet dans l'enceinte de Scholae. Il est géré par [Niko](https://microlinux.fr/).
C'est une sorte de "contrôle parental" si vous voulez, qui remplit essentiellement deux fonctions :

1. Empêcher les utilisateurs de surfer sur la face obscure du web,
2. Préserver la maigre bande passante en interdisant les sites qui consomment beaucoup trop de ressources (mises à jour, téléchargements, streaming, jeux en ligne, ...).

Cette configuration nécessite l'installation d'un certificat dans votre navigateur, que vous pouvez installer sur place.

## Comment accéder à Internet ?

Vous êtes tous libres d’utiliser Internet avec les machines de la salle info et avec vos
ordinateurs portables. Pour ce faire, vous devez impérativement installer le
certificat SSL de l’école sur vos machines.
Concrètement, il s’agit d’un fichier nommé certificat.der, que vous devez installer
soit dans votre navigateur web, soit directement dans votre système.

Voici une explication rapide pour tous les postes de la salle info, et plus
généralement pour tous ceux qui utilisent Mozilla Firefox pour surfer sur le web :

1. Lancez Mozilla Firefox.
2. Téléchargez le certificat à l’adresse http://192.168.10.254/certificat.der.
3. Ouvrez les Préférences de Firefox.
4. Ouvrez l’onglet Vie privée et sécurité.
5. Dans la section Certificats, cliquez sur Afficher les certificats.
6. Le Gestionnaire de certificats s’affiche.
7. Cliquez sur Importer.
8. Ouvrez le fichier certificat.der téléchargé.
9. Cochez les deux options Confirmer cette AC... et cliquez sur OK.

En dehors de cette explication succincte, la page http://192.168.10.254 rédigée par
mes soins contient des explications détaillées pour un certain nombre de systèmes
(Windows, macOS, Linux, Android, iOS) et de navigateurs web (Firefox, Chrome,
Safari, IE). Malheureusement, toutes ces configurations sont des cibles mouvantes, et
les ingénieurs système de chez Microsoft et Apple – pour ne citer que cet exemple –
adorent faire une refonte complète de l’ergonomie de leurs interfaces de
configuration1 à chaque nouvelle version. Pour vos smartphones, je vous conseille
fortement d’utiliser la 4G.


## Filtrage Internet

Toutes les machines sont reliées à Internet en accès libre, mais cet accès est filtré. Vous pouvez donc
utiliser l'accès au Web pour effectuer des recherches, lire la presse en ligne et gérer votre courrier
électronique via le webmail. En revanche, l'accès au côté obscur du Web est bloqué. Vous ne
pourrez donc pas télécharger la dernière saison de Cobra Kai, rejoindre le djihad en Syrie, adhérer
au parti nazi américain ou vous faire adopter par une cougar en ligne. C'est pas fun, je sais, mais la
loi française nous oblige à prendre ce genre de mesure. En revanche, il arrive parfois qu'un site
parfaitement licite soit bloqué. Dans ce cas, venez nous le signaler. Sachez également que les sites
que vous visitez et les fichiers que vous téléchargez laissent une trace sur le serveur proxy.
Ce filtage est également motivé par une autre raison purement pratique. Étant donné que la bande
passante de notre abonnement Internet est très modeste, j’ai coupé l’accès à tout ce qui est trop
gourmand en ressources. Du coup exit les mises à jour Microsoft et Apple, les sites de
téléchargement, les sites de streaming, les jeux en ligne, les serveurs de pubs, etc.

## Réseau wifi

L'école dispose d'un accès wifi libre en dehors des heures de travail, c'est-à-dire que vous pouvez
vous y connecter librement, sans authentification ou autre mot de passe. Bien évidemment, cet
accès est également soumis au filtrage Internet.

Dans certains cas, nous utilisons en système de secours une box Orange. Orange a une étrange notion des spams qui peut empêcher les mails @scholae.fr et @villa-figaret.fr de fonctionner avec vos logiciels habituels. Dans ce cas, il faut se connecter directement à l'un de ces deux sites 

- https://mail.scholae.fr
- https://mail.villa-figaret.fr
