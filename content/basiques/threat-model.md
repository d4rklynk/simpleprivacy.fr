---
title: "Le modèle de menace (ou comment bien démarrer) \U0001F3AF"
date: 2022-07-25
weight: 2
---
![Modèle de menace de Batman](/threat-model/threat-model-batman.png)

La modélisation des menaces (ou en anglais Threat Modeling) est un concept qui peut paraître compliqué aux premiers abords, mais qui s'avère être crucial pour comprendre ses besoins en matière de vie privée sur Internet.
Afin de mieux comprendre, je vais vous présenter deux exemples.

## L'exemple d'Alice

Alice possède un sac à dos, ce dernier contient :

- un livre
- des crayons
- un billet de 20 €

Elle habite dans une petite ville de campagne.
Elle se rend au café de sa ville chaque matin afin de lire son livre, elle pose son sac ouvert par terre comme à son habitude.
Après une heure de lecture, elle reprend son sac, et remarque que le billet de 20 a disparu, un pickpocket lui aura sûrement volé.

### Que peut-on en déduire de cette histoire ?

Les informations, possessions, données, ou toute autre entité que vous souhaitez protéger est appelé un **actif** (ici, le billet de 20 €) et le danger est appelé une **menace** (ici, le pickpocket).

5 choses essentielles sont à retenir :

1. Alice a perdu un billet de 20 €, c'est quand même beaucoup pour certains, mais elle n'a pas perdu tout son capital économique.
2. Un pickpocket le lui a volé, cela aurait pu être un voleur qui aurait pu prendre directement son sac, et donc perdre à la fois son billet et ses crayons.
3. Elle n'a pas eu de chance, elle réside dans une ville très calme, elle va à son café tous les jours. Les chances qu'il y ait un pickpocket à ce moment-là étaient quasi-nulles.
4. Elle peut toujours retirer un autre billet à la banque, ça l'embête, mais il lui reste beaucoup d'argent sur son compte en banque.
5. Elle aurait pu fermer son sac, mettre un cadenas dessus ou garder son sac sur ses genoux.

À partir de cette histoire, on peut établir un **modèle de menace** en 5 étapes :

1. Qu’est-ce qui vaut la peine d’être protégé ?

> Pour Alice, elle pouvait protéger son billet de 20 € et son livre, les crayons étant peu importants.

2. Contre qui les protéger ?

> Elle doit protéger ses affaires de potentiels voleurs ou pickpockets.

3. Quelle est la probabilité que ça arrive ?

> Pour Alice, la probabilité était quasi-nulle. Un pickpocket dans le café d'une ville de campagne, Alice a manqué de chance.

4. Quelle est l'ampleur des conséquences si j'échoue ?

> L'ampleur était minime pour Alice, elle n'a perdu que 20 €.

5. Quelles difficultés suis-je prêt à rencontrer pour prévenir ces conséquences ?

> Elle aurait pu en effet fermer son sac. Cependant, cela aurait été exagéré de mettre un cadenas dessus vu la probabilité qu'une telle situation puisse arriver.


Vous remarquerez qu'en réalité, on suit inconsciemment un modèle de menace. Vous allez acheter un sac normal en campagne, mais vous allez acheter des sacs à dos spéciaux (ouverture au niveau du dos) dans les grandes villes pour empêcher d'éventuels pickpockets. Vous ferez plus attention à votre téléphone dans les transports d'une grande ville qu'en campagne.

Maintenant que vous comprenez de quoi je parle, passons au deuxième exemple.

## L'exemple de Bob

Bob possède une valise pour ses vacances. Il contient notamment :

- Son PC portable
- Ses papiers
- De l'argent en monnaie courante

À l'aéroport, après l'atterrissage, sa valise est perdue parmi les autres. Impossible pour lui de la retrouver.

On remarque tout de suite qu'un **actif** peut devenir des **actifs**, on peut perdre beaucoup de choses différentes en une seule fois. Vous avez peut-être remarqué qu'il n'y a pas de "menaces", en fait si, mais ce n'est pas une personne. La menace dans cet exemple est l'organisation de l'aéroport, ou les gens qui s'occupent de retirer les bagages de la soute.

**Une menace est toute entité qui porte atteinte à vos actifs**, cela peut être un incendie brûlant tous vos documents, un autre événement naturel, une personne, une entreprise, etc.

Les 5 choses à retenir dans l'exemple de Bob sont :

1. Qu’est-ce qui vaut la peine d’être protégé ?

> Les actifs qu'il avait à protéger étaient le PC portable, ses papiers, et son argent en monnaie courante.

2. Contre qui les protéger ?

> La menace étant l'aéroport (ou l'organisation, ou les gens, etc.).

3. Quelle est la probabilité que ça arrive ?

> La probabilité que ça arrive est légère.

4. Quelle est l'ampleur des conséquences si j'échoue ?

> L'ampleur des conséquences est assez importante car il se retrouve dans un pays étranger, sans monnaie et sans papiers. Cela peut être plus ou moins facile de rentrer chez soi selon le pays où vous vous trouvez, mais même dans le meilleur des cas, vous vous retrouvez très embêté.
5. Quelles difficultés suis-je prêt à rencontrer pour prévenir ces conséquences ?

> Le fait qu'il ferme sa valise ou qu'il mette un cadenas dessus n'aurait pas pu prévenir ses conséquences. Il aurait pu cependant utiliser plusieurs valises, pour perdre moins d'actifs, mais cela complique le transport des valises de la maison de Bob vers l'aéroport. Une autre solution aurait pu être qu'il garde certains de ses actifs chez lui, tel que le PC portable, mais il en avait besoin pour ses vacances.

Ces 5 questions doivent être posées à chaque fois qu'un modèle de menace est établi, évidemment ce n'est pas immuable, le modèle de menace peut changer à cause de plusieurs facteurs, menaces technologiques, actifs plus importants/onéreux, etc.

Le principe de ces 5 questions est simple : **Se protéger des menaces potentielles, et non de toutes les menaces possibles.**

Cela demanderait beaucoup trop d'investissement, d'argent, et de temps pour pouvoir se protéger contre toutes les menaces.

Si on reprend les menaces d'Alice, en réalité on peut aller plus loin qu'un simple pickpocket. Imaginez qu'un incendie se déclare dans le café, qu'un tremblement de terre survient, ou que des soldats entrent dans le café car la guerre a éclaté entre son pays et un autre. C'est au revoir le sac à dos, peut-être même au revoir Alice.

Un autre exemple de modèle de menace sont les bâtiments. Au Japon, les bâtiments sont prévus pour résister à des séismes, puisque ce sont les menaces potentielles au Japon. On n'aura pas de ce genre de bâtiments en France.
Imaginez qu'à Brest on commence à construire des bâtiments résistants au feu, aux tornades, aux tsunamis, aux séismes, aux inondations, puis aux cambrioleurs, aux attentats, aux avions qui pourraient se crasher sur ces bâtiments, etc. Vous vous doutez bien que la plupart des solutions seraient inutiles, car il n'y a pas de séismes en Bretagne, ni de tornades ou de tsunamis. Cela prendrait trop de temps et d'argent, et si une menace est oubliée, tout le travail tomberait à l'eau. ***D'où l'importance de bien identifier les menaces potentielles.***

**Vous devez rester réaliste sur les menaces potentielles qui pourraient nuire à votre vie privée, ne minimisez pas les risques, mais ne maximisez par les menaces non plus (l'inverse est aussi vrai).**

## Un vrai exemple dans la vraie vie

Si je vous explique tout ça, c'est parce que quand les gens commencent à s'intéresser à la vie privée en ligne, ils se posent toujours les **mauvaises questions** :

- "Comment dois-je faire pour que Windows ne me piste pas ?"
- "Est-ce qu'Alexa est vraiment mauvaise pour votre vie privée ?"
- "Comment dois-je faire pour ne pas être pisté sur mon navigateur ?"
- "Dois-je changer mon Gmail pour Outlook ?"

Quand j'ai commencé à m'intéresser à tout ça, je me suis posé les mêmes questions, et je me retrouvais à avoir des paradoxes sur les choix que je prenais. Par exemple :

- Je modifiais mon Windows à l'extrême pour éviter d'être pisté.
- J'ai acheté une Alexa, parce que je me suis dit que c'était juste pour allumer mes lumières, et que ce n'était pas grave.
- J'ai installé [LineageOS](/basiques/smartphones/#aosp-et-firmware) sur mon téléphone pour éviter d'être pisté par Google, mais j'ai installé les applications Google, donc ça ne changeait rien.

Il ne faut pas se dire "Je n'aime pas les géants de la tech" ou "Je n'ai pas envie d'être pisté". Il faut réfléchir à comment ces entités peuvent vous pister, quelles sont les technologies qui permettent de faire ça, et comment vous pouvez faire pour réduire cette menace.

- J'ai donc commencé à me dire que je souhaitais **limiter la prise de  données par corrélation** aux services sur lesquels je me connectais. J'ai commencé à **mentir sur qui j'étais** puisque je me suis rendu compte que la plupart des services n'avaient pas besoin de savoir mon prénom, mon nom, mon sexe, etc. 
- Je me suis ensuite dit que je n'avais pas envie que **quiconque ait accès à mes données**, j'ai donc commencé à utiliser du [chiffrement de bout en bout](/basiques/instant-messengers/#le-chiffrement-de-bout-en-bout) pour les services cloud et les mails. J'utilise donc **Proton Drive** pour le **cloud**, et **Proton Mail** pour les **mails**. Puis pour la **communication** avec mes proches, je n'utilise plus que [Signal](/basiques/instant-messengers/#signal). J'ai acheté une Alexa, mais elle n'utilisait pas le chiffrement de bout en bout, je l'ai donc débranché, parce que les employés d'Amazon avaient accès à ma voix.
- Cependant, si je me connecte à mes comptes Google, Facebook, Instagram, etc, ils savent déjà qui je suis. J'ai donc limité le plus possible la collecte de données dans les paramètres de ces services. Mais comme la collecte de données reste inévitable, les menaces potentielles ne sont pas cette collecte de données, mais qu'un tiers ait accès à mon compte. J'ai donc commencé à sécuriser le plus possible mes comptes en utilisant des [mots de passe robustes](/basiques/password-managers) et en activant l'authentification à double facteur.
- Je me suis rendu compte également que la sécurité était tout aussi importante, car si je souhaite que personne n'ait accès à mes données, j'avais besoin de sécuriser un maximum mes appareils. Mon Windows n'était plus sécurisé car je l'avais beaucoup trop modifié. [LineageOS n'était absolument pas sécurisé](https://madaidans-insecurities.github.io/android.html#lineageos), etc.

En vous posant les bonnes questions, les réponses seront beaucoup plus claires, c'est pourquoi je vous explique sur mon site web comment fonctionnent certains services et certaines applications, et comment se prémunir d'éventuelles menaces, pour que vous sachiez quoi faire.

## Le modèle de menace sur Internet

![GAFAM](/threat-model/gafam.png)

Sur Internet, vos actifs sont vos données personnelles :

- Prénom/nom
- Âge
- Sexe
- Genre
- Intérêts personnels/politiques/religieux (basé sur vos recherches, vos communications, vos achats, etc.)
- Compte bancaire
- Opinions
- etc.

### Les géants de la tech ne sont pas la source du problème

L'erreur du débutant est de penser que les grosses entreprises de technologie, les GAFAM (Google, Amazon, Facebook, Microsoft) sont les menaces. C'est une mauvaise approche, exemple :
- Vous partagez vos photos de famille via Google Photos.
- Google a un accès à vos données, il les analyse et revend toute info potentielle à des tiers.

Vous allez vous dire qu'il y a pas photo (c'est un bon jeu de mots, avouez-le), c'est bien Google la menace. Non, car si vous changez pour un autre service, disons que j'en crée un que j'appelle `samsepi0l Cl0ud` :
- Vous mettez vos fichiers sur `samsepi0l Cl0ud`.
- J'ai toujours accès à vos données, mais je n'en fais rien, je ne les lis pas non plus.
- De plus en plus de gens décident d'utiliser mon service cloud.
- Je me dis que je peux me faire beaucoup plus d'argent, et je décide finalement de lire toutes vos données et de les revendre.

Je n'étais ni un géant de la tech, ni un GAFAM, mais j'ai voulu faire beaucoup plus de profit. Et le plus important : ***j'ai pu le faire parce que j'avais accès à vos données.***

La réelle menace, c'est que les données sont en clair sur les serveurs de ces entreprises, si j'avais implémenté du [chiffrement de bout en bout](/basiques/instant-messengers#le-chiffrement-de-bout-en-bout) sur mon service, j'aurais été incapable de lire vos données puisqu'elles auraient été illisibles sur mon serveur. Il n'y a que vous qui aurez pu avoir accès à vos fichiers, être capable de les lire, etc.

## Exemple de modèles

Je dirais qu'il y a 4 modèles de menaces différents concernant la vie privée sur Internet :
- Les fournisseurs de services qui espionnent ses utilisateurs
- [Le capitalisme de surveillance](https://fr.wikipedia.org/wiki/%C3%89conomie_de_la_surveillance)
- Informations publiques
- Les piratages de masse (tels que les virus, les applications malintentionnées, ...)

### Protéger votre vie privée des fournisseurs de services

Aujourd'hui, le fonctionnement basique d'un fournisseur de services consiste à garder les données en clair sur un serveur.

> En réalité, vos données sont chiffrées sur leurs serveurs, mais les fournisseurs détiennent la clé pour déchiffrer vos fichiers. Pour faire simple, le fournisseur voit en clair vos données, cependant si un hacker venait à compromettre un des serveurs, vos données seraient illisibles, car uniquement vous et le fournisseur avez la clé permettant de déchiffrer vos données. C'est comme si vous aviez un coffre-fort à la banque et que vous leur donniez la clé. Quand vous allez à la banque, vous leur demandez d'ouvrir votre coffre-fort, la banque vérifiera juste que c'est bien vous (mail et mot de passe) et vous ouvrira le coffre. Cependant, si un voleur arrive à voler la clé à la banquière, votre coffre est compromis, une situation similaire n'est pas impossible avec les fournisseurs de services.

Nos conversations privées par exemple sont en clair sur Discord, [Facebook Messenger](/basiques/instant-messengers/#facebook-messenger), [Telegram](/basiques/instant-messengers/#telegram) ou les SMS, tous les messages peuvent être lu par les fournisseurs eux-mêmes ou des tiers (comme des hackers par exemple).

### Les solutions

Vous pouvez prévenir ces conséquences en utilisant un service qui propose le chiffrement de bout en bout.

> Ce n'est plus la banquière qui a la clé, mais vous, et vous seul uniquement.

[Signal](https://www.signal.org/fr/#signal) est un bon exemple de service de messagerie qui propose un chiffrement de bout en bout, vous et votre destinataire uniquement avez connaissance du message.

> Les serveurs de Signal ne savent pas qui a écrit le message, ni ce qu'il y a dedans, ils savent juste à qui envoyer le message.

Proton Drive est un autre exemple de service qui propose un chiffrement de bout en bout (Proton Drive a été créé par Proton Mail), uniquement vous, avez accès à vos fichiers.

### Protéger votre vie privée du capitalisme de la surveillance

[Le capitalisme de surveillance](https://fr.wikipedia.org/wiki/%C3%89conomie_de_la_surveillance) est le champ économique qui tire profit de la surveillance numérique de masse.
Les exemples typiques sont le [scandale de Cambridge Analytica](https://www.frandroid.com/culture-tech/494669_cambridge-analytica-tout-comprendre-au-scandale-de-fuite-de-donnees-qui-secoue-facebook) (voir "The Great Hack" sur Netflix) ou les [révélations d'Edward Snowden](https://www.lemonde.fr/pixels/article/2020/09/03/un-programme-de-surveillance-telephonique-de-la-nsa-juge-illegal-en-appel_6050843_4408996.html), de grosses entreprises collectaient les informations personnelles des gens puis les redonner au gouvernement américain.
Afin de pister une personne, beaucoup de paramètres sont pris en compte, les plus courants sont :

- Votre adresse IP
- Les cookies de votre navigateur web
- Le [fingerprinting](https://www.cnil.fr/fr/definition/fingerprinting) (n'utilisez pas d'extension comme le propose la CNIL dans ce lien, c'est inutile)
- Les données que vous donnez aux sites web
- La corrélation des méthodes de payement (vous utilisez la même carte bancaire partout)

### Les solutions

La règle d'or : **Mentez**

J'utilise la Fnac comme exemple, mais c'est valable pour absolument **tout** sur Internet.

Est-ce que la Fnac a besoin de savoir que vous êtes une femme ou un homme ? Ont-ils réellement besoin de savoir votre âge ?
Absolument pas, réduisez le nombre d'informations requis au minimum.

Si vous le pouvez, ne créez pas de compte à la Fnac par exemple.

Si vous en avez déjà un, changez toutes les infos, choisissez non-binaire, homme, femme ou n'importe quoi d'autre dans la catégorie sexe, mettez que vous avez 75 ou 19 ans, dites que vous avez 4 enfants ou aucun (même si vous en avez ou pas), etc.
Faites-le partout, et changez les infos autant que possible.

> Un VPN peut-être une solution afin de cacher sa véritable IP... Mais je reviendrai à ce sujet plus tard...

Le but étant de ***séparer votre activité en ligne de votre réelle identité***.

### Limiter l'information publique

La meilleure manière de garder vos informations privées et de ne pas les mettre sur Internet en premier lieu.

Cependant, vous avez probablement des comptes en mode publique, comme Instagram, Facebook ou encore Twitter. Allez dans les paramètres et activez le mode "compte privé", cela empêchera que vous soyez dans les résultats des moteurs de recherche par exemple (ex : Google). Et vous devrez accepter manuellement les gens qui veulent voir votre compte (faites-le, même si vous souhaitez accepter tout le monde).

Encore une fois, ***omettez ou falsifiez vos informations*** le plus possible.

---

*Voir mes autres articles sur le sujet :*

- [Instagram : Limitez l'information publique et la collecte de données](/fiches/instagram)
- [Google : Limitez la collecte de données et sécurisez votre compte](/fiches/google)

---

### Se protéger des virus et des hackers

La vie privée sur Internet va de pair avec la sécurité. Si vous ne prenez pas en compte cet aspect, vous démarrez très mal.

> C'est bien de fermer les rideaux et de fermer votre porte, mais si les fenêtres s'ouvrent de l'extérieur ou que la porte n'as pas de serrure, vous pouvez très vite subir une violation de votre vie privée. Et tout ce que vous aviez entrepris pour protéger votre vie privée est réduite à néant par une simple porte.

En ce qui concerne les applications (qu'elles soient open source ou pas), on ne peut pas savoir si elles sont malveillantes ou si elles le deviendront un jour.

Je vous ***déconseille fortement*** d'utiliser des antivirus tiers comme Avast, Kasperky, McAfee, etc. [C'est inutile](https://privsec.dev/os/android-tips/#manage-android-permissions), voire [dangereux](https://privsec.dev/knowledge/badness-enumeration/#antiviruses), utilisez juste ce que vous propose votre système d'exploitation par défaut. Windows vous propose Microsoft Defender (ou anciennement appelé Windows Defender), utilisez uniquement celui-ci. La même chose s'applique pour macOS qui depuis [août 2022](https://eclecticlight.co/2022/08/30/macos-now-scans-for-malware-whenever-it-gets-a-chance/) propose un [antivirus intégré](https://support.apple.com/guide/security/protecting-against-malware-sec469d47bd8/web) (mais caché pour l'utilisateur). Et n'installez pas d'antivirus sur votre téléphone non plus !

Si vous avez acheté un PC sous Windows qui propose un autre antivirus par défaut (Avast, McAfee, AVG...), je ne peux que vous suggérer de le désactiver et d'utiliser Microsoft Defender à la place.

Un [chapitre](https://wonderfall.space/windows-hardening/#microsoft-defender-antivirus) sur ce problème a déjà été traité par [Wonderfall](https://wonderfall.space/). Je vous invite fortement à le consulter (article en français).

Les antivirus se basent sur le principe de [badness enumeration](https://privsec.dev/knowledge/badness-enumeration/#antiviruses) (littéralement : l'énumération du mal) qui est une méthode complètement dépassée et détachée de la réalité. L'antivirus est toujours en retard, des virus sont créés tous les jours, vous vous doutez bien que c'est impossible de tenir une liste ultra-précise de tous les virus possibles.

Il faut aussi comprendre que la "sécurité totale" n'existe pas, on parle de "très sécurisé" mais jamais de sécurité complète. Même les plus gros services, qui sont réputés pour être très sécurisés, possèdent leurs failles, comme Google, Facebook, Microsoft, Apple, etc. Mais des pays entiers peuvent également subir des fuites de données.

GrapheneOS est un bon exemple, c'est un système d'exploitation basé sur Android (le projet [AOSP](/basiques/smartphones/#aosp-et-firmware)) qui se veut être très sécurisé, mais vous vous doutez bien que si vous faites n'importe quoi avec, GrapheneOS ne pourra plus rien pour vous.

> Dites-vous que la sécurité est exactement comme une voiture, on peut faire des airbags, des ceintures de sécurité, des aides au freinage, etc. Mais si vous foncez à 150 km/h contre un mur, vous n'allez pas faire long feu 😅️. Même avec la voiture la plus sécurisée du monde.

### Les solutions

La meilleure technique dans ce cas est, si vous avez la chance d'avoir plusieurs PC, d'utiliser vos appareils à des fins différentes. Par exemple, si vous avez deux ordinateurs, un fixe et un portable, utilisez le fixe pour vos fins personnelles, et utilisez le portable pour vos fins professionnelles.

Ça s'appelle le cloisonnement.

Ne partagez pas votre PC, et au pire des cas, créez toujours une session dédiée à cette personne.

## Mauvaises pratiques

Les **erreurs** de débutant les plus communes sont de :

- Se concentrer uniquement sur les GAFAM, et non les [fournisseurs de services dans leur ensemble](#les-géants-de-la-tech-ne-sont-pas-la-source-du-problème).
- Faire énormément confiance à la Politique de Confidentialité, alors que cette politique peut être violable à tout moment.
- Faire aveuglément confiance à un autre service juste parce que ce n'est pas un géant de la tech.
- Faire aveuglément confiance aux solutions open source.

[Comme dit plus haut](#les-géants-de-la-tech-ne-sont-pas-la-source-du-problème), essayez de déterminer le vrai problème de fond. Si vous n'aimez pas Google Drive parce qu'ils ont un accès complet à vos données, le problème n'est pas Google, mais le manque de [chiffrement de bout en bout](/basiques/instant-messengers.md/#le-chiffrement-de-bout-en-bout). Si vous passez de Google Drive à OneDrive par exemple, le problème reste exactement le même : Microsoft (OneDrive) a accès à vos données.

Alors qu'en chiffrant vos fichiers avant de les transférer sur votre service cloud préféré, ou plus simple encore, d'utiliser un service qui propose un chiffrement de bout en bout par défaut comme [Proton Drive](https://proton.me/fr/drive). Là, vous réglez le vrai problème de fond.

En ce qui concerne les applications open source, ce n'est pas parce qu'elles sont open source qu'elles respectent votre vie privée ou qu'elles sont très sécurisées. C'est mieux d'utiliser un logiciel open source, car d'autres personnes ont revu le code et savent ce que le programme fait, mais rien nous dit que son alternative propriétaire (une autre application du même style qui ne serait pas open source) n'est pas plus sécurisée.

---

## Crédits

- 🇬🇧️ [Threat Model - PrivSec.Dev](https://privsec.dev/knowledge/threat-modeling/) *(j'ai le même thème que son site web car c'est un thème publique et gratuit, ne soyez pas étonné)*
- 🇬🇧️ [Badness Enumeration - PrivSec.dev](https://privsec.dev/knowledge/badness-enumeration/)
- 🇬🇧️ [10 dumbest ideas in privacy communities - rhbik5](https://www.reddit.com/r/PrivacyGuides/comments/rhbik5/10_dumbest_ideas_in_privacy_communities/)
- 🇬🇧️ [The Six Dumbest Ideas in Computer Security](https://www.ranum.com/security/computer_security/editorials/dumb/index.html)
- 🇬🇧️ [Android Tips - PrivSec.dev](https://privsec.dev/os/android-tips/)
- 🇫🇷️ [Windows 10 - Chapitre sur Microsoft Defender - Wonderfall](https://wonderfall.space/windows-hardening/#microsoft-defender-antivirus)
- 🇫🇷️ [Votre plan de sécurité - EFF](https://ssd.eff.org/fr/module/votre-plan-de-s%C3%A9curit%C3%A9)
