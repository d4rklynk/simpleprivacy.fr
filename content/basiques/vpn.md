---
title: "Les VPNs"
---

![vpn-cover.jpg](/vpn/vpn-cover.jpg)

Aaah les VPN, la solution ultime afin d'être anonyme en ligne !
Quelle blague...

## C'est quoi un VPN ?

Commençons par le commencement voulez-vous ?

Un Virtual Private Network (VPN) ou Réseau Privé Virtuel en français est une technologie permettant de vous connecter à un autre réseau local.

![local-network.png](/vpn/local-network.png)

Voici deux réseaux locaux dans l'image ci-dessus. Un réseau local est un petit réseau qui regroupe un ensemble de machines. Typiquement, quand vous êtes chez vous, vous êtes dans un réseau local. Un réseau local n'est pas obligatoirement connecté à Internet, mais les machines à l'intérieur sont connectées entre elles, c'est pourquoi vous pouvez imprimer chez vous et non chez l'imprimante de votre voisin.

Imaginons que vous êtes dans le réseau local numéro 1 (chez vous) et qu'un de vos amis possède un serveur de fichiers chez lui dans le réseau local numéro 2. Votre ami vous dit qu'il a plein de photos et de vidéos qu'il aimerait vous partager.

> *Un serveur de fichiers est un ordinateur qui stocke des fichiers et les rend accessibles à d'autres ordinateurs sur un réseau.*

Dans le cas actuel, vous ne pouvez pas accéder à son serveur car il est dans un autre réseau local que le vôtre. Le seul moyen d'accéder à son serveur avec la configuration actuelle est de vous déplacer chez lui.

Ou alors, vous pouvez utiliser un VPN pour accéder au réseau local de votre ami !

![vpn-client-serveur.png](/vpn/vpn-client-serveur.png)

Ce VPN n'est pas du tout le même que les VPN pour le grand public (NordVPN, ExpressVPN, etc). Ici, c'est un VPN "fait-maison", car les deux plus gros protocoles connues pour créer un serveur VPN sont [OpenVPN](https://openvpn.net/) et [WireGuard](https://www.wireguard.com/), ils sont gratuits et open-source. N'importe qui peut donc configurer un VPN gratuitement afin de se connecter à un autre réseau comme dans notre exemple.

Dans cette configuration, on a un client (VPN) et un serveur (VPN), le client se connecte au serveur distant (en passant par Internet) afin d'accéder aux ressources du réseau numéro 2. Le client (du réseau numéro 1) aura donc accès à toutes les ressources du réseau distant (réseau numéro 2), mais le réseau distant ne peut pas accéder au ressources du réseau du client.

Évidemment, et c'est là tout le principe, tout la connexion est chiffrée (du poste du client jusqu'au serveur VPN du réseau distant).

> Contrairement à ce que vous pourriez penser, la configuration d'un VPN est très simple. D'ailleurs, vous pouvez même créer un serveur VPN avec votre Freebox si vous en avez une.

## La différence entre un VPN "maison" et les VPN grand public

WIP
Faire une vidéo des logs d'un VPN (setup un serveur et afficher les logs)

## Pourquoi c'est une mauvaise idée d'héberger votre propre VPN

## Pourquoi y a-t-il autant de fournisseurs de VPNs ?

Parce qu'un VPN, c'est de l'argent gratuit pour la personne qui le gère. C'est juste un fichier de configuration à mettre en place et un client à développer afin que les utilisateurs de tout type puissent s'y connecter facilement. Vous louez plusieurs serveurs, vous configurez votre serveur VPN sur chaque, vous louez votre prestation et le tour est joué.

## Ça veut dire quoi no-log ?
## Les faux arguments des vendeurs
### C'est plus sécurisé !

> Votre connexion est sécurisée avec des protocoles militaires !

Alors déjà, encore heureux que la connexion est sécurisée parce que c'est le principe même du VPN : "Accéder à un autre réseau de manière sécurisée".

Ensuite quand ils parlent de protocoles militaires, c'est juste des protocoles standards que tout le monde utilise aujourd'hui. Sinon dans ce cas, mon site web aussi utilise du chiffrement militaire.

Pour avoir un transport sécurisé sur Internet, vous avez juste à aller sur votre navigateur web préféré, accéder à n'importe quel site web en HTTPS, et voilà, votre connexion est sécurisé, parce que c'est ça qui importe. De toute façon, HTTPS est devenu un critère de référence sur Google il y a des années de cela, donc si vous souhaitez que votre site web soit visible sur Google, il doit obligatoirement proposer du HTTPS.

### Votre FAI ne pourra plus savoir ce que vous faites

Votre trafic est chiffré jusqu'au serveur de votre fournisseur VPN, mais une fois arrivé sur ce serveur, votre trafic est déchiffré afin que vous puissiez accéder à vos sites web préférés. En effet, votre FAI sait juste que vous utilisez un VPN mais ne sait pas ce que vous faites, mais le revers de la médaille, c'est que c'est maintenant votre fournisseur qui sait tout ! Yes...
Au lieu de donner tout votre trafic Internet à votre FAI, vous le donnez à votre fournisseur de VPN !

### Votre gouvernement ne pourra plus vous espionner

WIP

## Le top 10 des meilleurs VPNs de ce mois-ci !

Vous avez du voir ce genre de liste un nombre incalculable de fois. 

Et bien en fait, ces listes des meilleurs VPN du mois ou de l'année en cours sont réfléchies. En effet, ils prennent les meilleurs personnes en sécurité pour créer ce top 10... Non, vous vous doutez bien que non. C'est déguisé en comparatif ou top 10 des meilleurs VPNs, mais en réalité, ce sont juste des amas de lien d'affiliation pour se faire un maximum d'argent. Les personnes qui écrivent ces comparatifs se fichent de savoir quel VPN vous allez prendre. Car tant que vous cliquez sur un de leurs liens d'affiliations, ils se feront de l'argent.

J'ai pris le premier lien que je voyais et regardez comme c'est beau :

![cnet-lien.png](/vpn/cnet-lien.png)

Quand je passe la souris sur le bouton rouge "**VOIR LES OFFRES NORDVPN**", le lien affiché par le navigateur en bas à gauche contient les mots `aff`, `offer_id` et plein d'autres. Bref, cec sont juste des listes pour faire de l'argent, laissez-moi vous simplifier la vie et vous montrez ce que vous êtes censé voir quand vous lisez un de soi-disant "comparatifs" :

- VPN n°1 - Lien d'affiliation qui va me donner plein d'argent
- VPN n°2 - Lien d'affiliation qui va me donner plein d'argent
- VPN n°3 - Lien d'affiliation qui va me donner plein d'argent
- VPN n°4 - Lien d'affiliation qui va me donner plein d'argent
- VPN n°5 - Lien d'affiliation qui va me donner plein d'argent

Voilà, cette liste est, attention, revue par des experts dans le milieu.

C'est valable sur 99,99% des sites que vous verrez. Afin de savoir si les liens sont affiliés, vous avez juste à passer la souris sur le soi-disant bouton qui ramène vers le site, si le lien est super long comme ici, il est fort probable que ce soit un lien d'affiliation.
Si vous souhaitez vraiment choisir un vrai VPN qui respecte vraiment votre vie privée, je vous suggère de regarder sur [PrivacyGuides](https://www.privacyguides.org/fr/vpn/) ou [les alternatives](/alternatives/providers/#les-vpns) que je propose (qui sont évidemment non affiliés).

##  Mais quelle est la réelle utilité ?

Un VPN (grand public) va essentiellement faire 3 choses :

- Avoir une adresse IP différente de la vôtre et partagée par plusieurs personnes (car plusieurs personne se connectent sur le même serveur que vous). Ce qui a le gros avantage de se fondre dans la masse.

## Avez-vous vraiment besoin d'un VPN ?