---
title: "Les VPNs 🌍️"
date: 2023-06-09
---

![vpn-cover.jpg](/vpn/vpn-cover.jpg)

Aaah les VPN, la solution ultime afin d'être anonyme en ligne !
Quelle blague...

## C'est quoi un VPN ?

Commençons par le commencement.

Un Virtual Private Network (VPN) ou Réseau Privé Virtuel en français est une technologie permettant de vous connecter à un autre réseau local.

![local-network.png](/vpn/local-network.png)

Voici deux réseaux locaux dans l'image ci-dessus. Un réseau local est un petit réseau qui regroupe un ensemble de machines. Typiquement, quand vous êtes chez vous, vous êtes dans un réseau local. Un réseau local est souvent connecté à Internet, mais ce n'est pas systématiquement le cas. Cela va de soi, votre réseau local chez vous est connecté à Internet, sinon vous ne pourriez pas lire mon article 😄️. Cependant, les machines à l'intérieur sont connectées entre elles (et uniquement dans ce réseau), c'est pourquoi vous pouvez imprimer chez vous et non chez l'imprimante de votre voisin (car c'est un autre réseau local).

Imaginons que vous êtes dans le réseau local numéro 1 (chez vous) et qu'un de vos amis possède un serveur de fichiers chez lui dans le réseau local numéro 2. Votre ami vous dit qu'il a plein de photos et de vidéos qu'il aimerait vous partager.

> *Un serveur de fichiers est un ordinateur qui stocke des fichiers (photos, vidéos, documents, etc.) et les rend accessibles à d'autres ordinateurs sur un réseau.*

Dans le cas actuel, vous ne pouvez pas accéder à son serveur car il est dans un autre réseau local que le vôtre. Le seul moyen d'accéder à son serveur avec la configuration actuelle est de vous déplacer chez lui.

Ou alors justement, vous pouvez utiliser un VPN pour accéder au réseau local de votre ami !

![vpn-client-serveur.png](/vpn/vpn-client-serveur.png)

Ce VPN n'est pas du tout le même que les VPN pour le grand public (NordVPN, ExpressVPN, CyberGhost, etc). Ici, c'est un VPN "fait-maison". Les deux plus gros protocoles connus pour créer un serveur VPN sont [OpenVPN](https://openvpn.net/) et [WireGuard](https://www.wireguard.com/), ils sont gratuits et open-source. Par ailleurs, la quasi-totalité des VPNs "grand public" utilisent ces deux protocoles. N'importe qui peut donc configurer un VPN gratuitement afin de se connecter à un autre réseau comme dans notre exemple.

Dans cette configuration, on a un client (VPN) et un serveur (VPN), le client se connecte au serveur distant (en passant par Internet) afin d'accéder aux ressources du réseau numéro 2. Le client (du réseau numéro 1) aura donc accès à toutes les ressources du réseau distant (réseau numéro 2), mais le réseau distant ne peut pas accéder au ressources du réseau du client.

Évidemment, et c'est là tout le principe, tout la connexion est chiffrée (du poste du client jusqu'au serveur VPN du réseau distant).

> Contrairement à ce que vous pourriez penser, la configuration d'un VPN est très simple. D'ailleurs, vous pouvez même créer un serveur VPN avec votre Freebox par exemple.

## Pourquoi y a-t-il autant de fournisseurs de VPNs ?

Parce que c'est hyper rentable. C'est juste un fichier de configuration à mettre en place et un client à développer afin que les utilisateurs de tout type puissent s'y connecter facilement. Vous louez plusieurs serveurs, vous configurez votre serveur VPN sur chaque, vous louez votre prestation et le tour est joué.

## Ça veut dire quoi no-log ?

Quand on parle de no-log, on parle de ce qu'on appelle les journaux d'activité. C'est un fichier ou un ensemble de fichiers textes dans lequel se trouve pléthore de messages générés par un programme ou un système. C'est absolument nécessaire car c'est ce qui nous permet de tracer les événements d'une machine afin de retrouver certains problèmes. Les logs sont faites pour faciliter grandement la surveillance, l'analyse et le dépannage.

Dans le cas d'un VPN, quand on parle de no-log, ce n'est pas de ce type de logs dont on parle. Ici, ce sont les logs d'informations personnelles, telles que votre IP, les sites que vous visitez, la durée de session, ou votre emplacement.

Typiquement, les VPNs gratuits (sauf Proton VPN qui est un cas unique) vont analyser votre trafic, votre IP, votre durée de session, les sites que vous visitez pour revendre vos données afin de vous envoyer de la publicité personnalisée. Eh ben oui, vous aviez cru quoi ? 😮‍💨️

En général, no-log veut dire ceux-ci :

- Les sites que vous visitez ne sont pas enregistrés
- Votre IP n'est pas enregistré (ce n'est pas enregistré, mais un fournisseur VPN connaîtra toujours votre IP réel)
- Le temps de session n'est pas enregistré (et encore, ça dépend)

Je tiens à noter que **quelque soit** votre fournisseur VPN, si la justice demande des informations vous concernant, ils ne vont pas enfreindre la loi pour vous protéger, et c'est tout à fait normal !

Dans la mesure on rien n'est enregistré, votre fournisseur VPN ne pourra rien donner à la justice, si elle le lui demande. Cependant, il est important de noter que si la justice demande à votre fournisseur de commencer à vous log (ou "journaliser" en bon français) (c'est à dire enregistrer les sites sur lesquels vous vous connectez, votre IP, etc...), votre fournisseur le fera sans hésiter. Un VPN n'est pas fait pour être anonyme en ligne contrairement à ce que d'autres entreprises bien connues du grand public veulent vous faire croire.

## Les faux arguments des vendeurs
### C'est plus sécurisé !

> Votre connexion est sécurisée avec des protocoles militaires !

Alors déjà, encore heureux que la connexion est sécurisée parce que c'est le principe même du VPN : "Accéder à un autre réseau de manière sécurisée".

Ensuite quand ils parlent de protocoles militaires, c'est juste des protocoles standards que tout le monde utilise aujourd'hui. Sinon dans ce cas, mon site web aussi utilise du chiffrement militaire.

Pour avoir un transport sécurisé sur Internet, vous avez juste à aller sur votre navigateur web préféré, accéder à n'importe quel site web en HTTPS, et voilà, votre connexion est sécurisée, parce que c'est ça qui importe. De toute façon, HTTPS est devenu un critère de référencement sur Google [il y a des années de cela](https://developers.google.com/search/blog/2014/08/https-as-ranking-signal), donc si vous souhaitez que votre site web soit visible sur Google, il doit obligatoirement proposer du HTTPS.

Et puis aujourd'hui, [95%](https://transparencyreport.google.com/https/overview?hl=fr) des sites web visibles par Google sont en HTTPS :)

![googlehttps.png](/vpn/googlehttps.png)

### Votre FAI ne pourra plus savoir ce que vous faites

En effet, comme votre trafic Internet est chiffré jusqu'au serveur de votre fournisseur VPN, votre trafic passe certes par votre FAI (Fournisseur d'Accès à Internet -> Orange, Free, SFR, etc.) mais est illisible par ce dernier. Cependant, une fois que vous êtes connecté sur le serveur de votre fournisseur VPN, votre trafic est déchiffré afin que vous puissiez accéder à vos sites web préférés. En effet, votre FAI sait juste que vous utilisez un VPN mais ne sait pas ce que vous faites, mais le revers de la médaille, c'est que c'est maintenant votre fournisseur VPN qui sait tout ! Yes...
Au lieu de donner tout votre trafic Internet à votre FAI, vous le donnez à votre fournisseur de VPN !

Il est donc important de ne pas prendre n'importe quoi comme VPN, car vous devez lui faire confiance de ne pas enregistrer tout votre trafic Internet.

### Votre gouvernement ne pourra plus vous espionner

Ils ne pourront pas savoir quels sites vous visitez, mais ils peuvent tout de même vous reconnaître à vos habitudes de navigation, les sites sur lesquels vous vous connectez, etc...

En effet si vous vous connectez sur vos sites web habituels, quel est l’intérêt d'utiliser un VPN ???

Votre fournisseur de VPN est également soumis à la loi, ils sont donc obligés légalement de fournir ces informations.

Si vous vous trouvez dans un pays très restrictif, vous allez plutôt utiliser [Tor Browser](https://www.torproject.org/), c'est bien plus efficace pour lutter contre l'espionnage de votre gouvernement.

Rappelez-vous également les données personnelles que vous avez donné à votre fournisseur quand vous vous êtes inscrit 😁️. Petite piqûre de rappel si vous avez oublié :

- Votre adresse mail
- Votre carte bancaire
- Votre localisation
- Votre nom
- Votre prénom
- Votre âge

Donc si le gouvernement demande au VPN d'enregistrer vos données, je vous garantis que le fournisseur le fera, et c'est normal (et c'est déjà arrivé plusieurs fois, même [chez Proton](https://proton.me/blog/climate-activist-arrest) (l'activiste était un squatteur qui s'introduisait chez les gens)).

## Le top 10 des meilleurs VPNs de ce mois-ci !

Vous avez du voir ce genre de liste un nombre incalculable de fois. 

Et bien en fait, ces listes des meilleurs VPN du mois ou de l'année en cours sont réfléchies. En effet, ils prennent les meilleurs personnes en sécurité pour créer ce top 10... Non, vous vous doutez bien que non. C'est déguisé en comparatif ou top 10 des meilleurs VPNs, mais en réalité, ce sont juste des amas de liens d'affiliation pour se faire un maximum d'argent. Les personnes qui écrivent ces comparatifs se fichent de savoir quel VPN vous allez prendre. Car tant que vous cliquez sur un de leurs liens d'affiliation, ils se feront de l'argent.

J'ai pris le premier lien que je voyais et regardez comme c'est beau :

![cnet-lien.png](/vpn/cnet-lien.png)

Quand je passe la souris sur le bouton rouge "**VOIR LES OFFRES NORDVPN**", le lien affiché par le navigateur en bas à gauche contient les mots `aff`, `offer_id` et plein d'autres. Bref, ce sont juste des listes pour faire de l'argent, laissez-moi vous simplifier la vie et vous montrez ce que vous êtes censé voir quand vous lisez un de ces prétendus "comparatifs" :

- VPN n°1 - Lien d'affiliation qui va nous rapporter plein d'argent
- VPN n°2 - Lien d'affiliation qui va nous rapporter plein d'argent
- VPN n°3 - Lien d'affiliation qui va nous rapporter plein d'argent
- VPN n°4 - Lien d'affiliation qui va nous rapporter plein d'argent
- VPN n°5 - Lien d'affiliation qui va nous rapporter plein d'argent

Voilà, cette liste est, attention, revue par des experts dans le milieu.

De toute évidence, la liste n'est pas ordonné selon quel VPN est le meilleur, mais selon le montant que le fournisseur de VPN a payé :)

Qu'on soit clair, on ne parle pas ici d'une conspiration mais d'un business model.

C'est valable sur 99,99% des sites que vous verrez. Afin de savoir si les liens sont affiliés, vous avez juste à passer la souris sur le soi-disant bouton qui ramène vers le site, si le lien est super long comme ici, il est fort probable que ce soit un lien d'affiliation.
Si vous souhaitez *vraiment* choisir un *vrai* VPN qui respecte *vraiment* votre vie privée, je vous suggère de regarder sur [PrivacyGuides](https://www.privacyguides.org/fr/vpn/) ou [les alternatives](/alternatives/providers/#les-vpns) que je propose (qui sont évidemment non affiliés).

## Pourquoi c'est une mauvaise idée d'héberger votre propre VPN

Un des avantages d'un VPN et de recevoir une IP partagée avec d'autres personnes, cela permet de vous fondre dans la masse.

Si vous hébergez votre propre VPN sur un serveur distant que vous avez loué, vous utiliserez toujours la même IP, donc vous aurez rien réglé du tout.

Pour imager un peu, c'est comme si vous portiez le même masque tous les jours pour aller n'importe où, même si on ne connaît pas votre visage, on saura qui vous êtes.

## Mais quelle est la réelle utilité ?

Un VPN (grand public) va essentiellement faire 3 choses :

- Vous attribuer une adresse IP différente de la vôtre (celle de votre box) et partagée par plusieurs personnes (car plusieurs personne se connectent sur le même serveur que vous). Ce qui a le gros avantage de vous faire fondre dans la masse.
- Mieux vous protéger dans les réseaux publics (comme le Wifi de chez McDonald par exemple). Mais franchement, il n'y a plus aucun intérêt puisque la majorité des gens utilise les données mobiles.
- Cacher votre IP lors de téléchargement de fichier torrent. Car quand vous téléchargez un fichier torrent, votre IP est visible par les seeders (ceux qui mettent à disposition le fichier), et évidemment, une fois ce fichier téléchargé, vous devenez seeder automatiquement, et donc votre IP est visible par tous les leechers (ceux qui téléchargent).

---

Aparté : le torrent (ou P2P pour "peer to peer") est totalement légal. Ce qui illégal en revanche est le partage de fichier qui ne vous appartient pas (comme les films, les séries, les livres etc.).

Vous pouvez consulter [Service-Public.fr](https://www.service-public.fr/particuliers/vosdroits/F32108) pour comprendre les textes de loi concernant le téléchargement illégal.

---

## Avez-vous vraiment besoin d'un VPN ?

Version courte : non.

Version longue : non, vous n'en avez pas besoin :)

Plus sérieusement, si vous souhaitez cacher votre IP lors de téléchargement de torrent ou si vous avez plus confiance en votre fournisseur VPN que votre FAI, alors vous pouvez prendre un VPN. Sinon, votre IP sera visible par ceux qui vous partage le fichier torrent ou ceux qui téléchargent le fichier que vous partagez. 

Pour ce qui est du cas de regarder du contenu vidéo aux États-Unis à partir de la France, ça fonctionne, mais gardez en tête que beaucoup de services de VOD (Netflix, Disney+, Prime Video, etc...) bloquent les IPs des serveurs venant de fournisseurs de VPNs. Donc une minorité des serveurs de votre fournisseur fonctionnera, évidemment, les fournisseurs achètent sans cesse de nouveaux serveurs (et donc par extension de nouvelles IP), c'est le jeu du chat et la souris. Pour faire simple, oui ça marche quelque soit le VPN (et ne croyez pas dur comme fer qu'un VPN fonctionnera **systématiquement** pour les services de VOD quoi que dise le vendeur).

Si vous décidez de choisir un VPN, je vous conseille de regarder [les alternatives](/alternatives/providers) que je propose (basé sur les [recommandations de PrivacyGuides](https://www.privacyguides.org/fr/vpn/)).

Je vous conseille de lire l'article de Wonderfall qui est très clair sur ce sujet. Mon article est "une entrée en la matière" au sien de toute manière.

## En savoir plus & crédits
- 🇫🇷️ [Les VPNs et leur mésusage - Wonderfall](https://web.archive.org/web/20230204125417/https://wonderfall.space/vpn-mesusage/) (à lire absolument !)
- 🇬🇧️ [Commercial VPN Use Cases](https://privsec.dev/posts/proxies/commercial-vpn-use-cases/) (’ai le même thème que son site web car c’est un thème publique et gratuit, ne soyez pas étonné)
- 🇫🇷️ [Services VPN - PrivacyGuides](https://www.privacyguides.org/fr/vpn/)
- 🇫🇷️ [Introduction aux VPNs - PrivacyGuides](https://www.privacyguides.org/fr/basics/vpn-overview/)
- 🇬🇧️ [DoIneedaVPN?](https://www.doineedavpn.com/) (certes en anglais, mais je vous conseille quand même d'y jeter un œil)
- 🇬🇧️ [VPN - a Very Precarious Narrative - Dennis Schubert](https://overengineer.dev/blog/2019/04/08/very-precarious-narrative.html)
- 🇬🇧️ [The Trouble with VPN and Privacy Review Sites - Jonah](https://blog.privacyguides.org/2019/11/20/the-trouble-with-vpn-and-privacy-review-sites/)