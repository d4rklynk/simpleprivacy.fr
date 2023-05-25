---
title: "Les smartphones \U0001f4f1"
date: 2022-08-07
weight: 4
---

![android](/smartphones/android.jpg)

Les smartphones sont des éponges à données, ils ont accès à beaucoup d'informations qu'on aimerait garder privées.

Cependant les smartphones (IOS et Android) sont bien plus sécurisés que les systèmes d'exploitation de bureau (Windows, Linux, macOS).
Vous avez remarqué par exemple qu'il y a un système de permission sur les smartphones qu'il n'y a pas sur les PC. Vous savez, les fenêtres qui s'affichent "Autoriser l'accès la position" ou "Autoriser l'accès à la caméra".


## Recommandations

Pour les smartphones, je vous recommande uniquement un [iPhone](https://wonderfall.space/modele-securite-mobile/#ios-chez-apple-la-prison-dor-e) ou un [Google Pixel](https://wonderfall.space/modele-securite-mobile/#google-pixel-android-done-right).

N'achetez **PAS** de Google Pixel chez votre fournisseur d'accès à Internet (Orange, Free, SFR, Bouygues). Le téléphone est bloqué et vous ne pouvez pas déverrouiller le bootloader comme expliqué plus loin dans [le chapitre dédié](#bootloader). Achetez **toujours** votre téléphone dans les magasins comme la Fnac, Boulanger, Amazon, etc.

Alors oui, je vous voir venir, mais si je vous recommande uniquement ces deux smartphones, c'est parce qu'ils sont les plus sécurisés du marché. Par exemple, vous pouvez mettre un code PIN à 4 chiffres sur ces téléphones (iPhone et Google Pixel), que ça prendrait des dizaines d'années à cracker (normalement, ça prend beaucoup moins de temps sur d'autres marques de téléphones).

Les Google Pixel, à partir du 6, ont [**5 ans de support**](https://support.google.com/pixelphone/answer/4457705?hl=fr#zippy=%2Ct%C3%A9l%C3%A9phones-pixel-et-versions-ult%C3%A9rieures) minimum.

Je vous épargne les détails techniques, mais pour faire très simple, les Google Pixel ne sont pas juste "un peu mieux sécurisés" que les autres marques, ils sont ***excellents en terme de sécurité.***
Je vous conseille donc très fortement de ne rester qu'avec un Google Pixel.

- [Google Pixel : Android done right - Wonderfall](https://wonderfall.space/modele-securite-mobile/#google-pixel-android-done-right) (français)
- [iOS : chez Apple, la prison dorée - Wonderfall](https://wonderfall.space/modele-securite-mobile/#ios-chez-apple-la-prison-dor-e) (français)
- [Google Pixel - PrivacyGuides](https://www.privacyguides.org/android/#google-pixel) (anglais)
- [Recommended Phones - PrivSec.dev](https://privsec.dev/os/android-tips/#recommended-phones) (anglais)

### Le problème de confiance

Il faut comprendre également que sur tous les smartphones Android qui contiennent les applications Google, vous avez une application appelée "`Services Google Play`". Cette application permet de faire beaucoup de choses, cependant, elle a accès à toutes les permissions du téléphone, même les plus sensibles, et sont irrévocables. C'est à cause de cette application que les problèmes de vie privée apparaissent. Android en lui-même n'est pas un problème, c'est l'ajout des applications de Google, et notamment des "`Services Google Play`" qui fait d'Android un cauchemar pour votre vie privée.

Si vous achetez un Samsung par exemple, cela veut dire que vous faites confiance à Google (à cause des `Services Google Play`) **ET** à Samsung pour vos données. Il est donc logique de réduire cette confiance à une seule entité et donc de prendre un Google Pixel.

## Sécurité


### AOSP et firmware

Je vous conseille de prendre un smartphone neuf, c'est à dire encore supporté par le constructeur, voici pourquoi : 

Deux types de mises à jour sont à faire sur un matériel informatique :

- la partie **logicielle**
- la partie **firmware**

La partie **logicielle** est le **système d'exploitation**, donc Android. Mais cela s'applique également à IOS et aux PC avec Windows, MacOS, Linux, ChromeOS, etc. La partie **firmware**, également appelée micrologicielle en français, est un mini-système d'exploitation pour les composants du matériel (la carte mère, la carte réseau, etc.). Ce n'est pas comme un pilote pour ceux ou celles qui se poseraient la question. Pour faire très simple, le firmware est le manuel d'utilisation des composants pour le système d'exploitation.

Je vais rapidement vous expliquer Android pour que vous compreniez bien. Voici un schéma qui vous explique le projet **AOSP** :

![AOSP schéma](/smartphones/aosp.png#center)

**AOSP** signifie **Android Open Source Project**, c'est le cœur de tous les téléphones Android aujourd'hui, AOSP à lui tout seul est très limité : vous n'avez pas d'applications Google par exemple. Comme ce projet est open source (mais détenu par Google) beaucoup de marques (toutes celles qui ne sont pas Apple, donc Samsung, Xiaomi, Huawei, OnePlus, Pocco, et j'en passe) vont prendre le code d'AOSP et le modifier un peu à leur sauce. C'est ce qu'on appelle la **surcouche Android**. **LineageOS** est une surcouche Android développée par des bénévoles.

> ***Quand on parle d'Android, on parle en réalité d'AOSP.***

La surcouche de Samsung par exemple, s'appelle **OneUI**, celle de OnePlus, **OxygenOS**, et celle de Xiaomi s'appelle **MIUI**. Cela fait toujours parti du système d'exploitation, ce ne sont pas des logiciels. 

Cependant, si AOSP est open source, les surcouches ne le sont pas forcément ! LineageOS est une surcouche open source par exemple, mais MIUI ne l'est pas !

> On parle de surcouche, mais en réalité, les constructeurs prennent le projet AOSP pour le modifier selon leurs besoins puis ajouter leurs programmes, leurs fonctionnalités, etc. Ce sont ces modifications et ces ajouts qui sont appellés la surcouche. 

> Dites-vous qu'AOSP est comme une recette de cuisine, tout le monde connait cette recette, mais certains cuisiniers ajouteront quelques épices ou d'autres ingrédients secrets. Donc oui vous connaissez précisément la recette de base, mais non, vous n'en savez pas plus sur les ingrédients ajoutés. Une surcouche tel que GrapheneOS est open source, on connait donc les ingrédients ajoutés.

Comprenez bien que si vous souhaitez installer LineageOS sur votre téléphone, cela veut dire que vous supprimez le système d'exploitation de votre téléphone. En gros, si vous allumez votre téléphone après avoir supprimé le système d'exploitation de Samsung par exemple, vous ne pourrez plus démarrer votre téléphone, car il n'y aura rien à démarrer ! Sauf si vous installez LineageOS juste après, évidemment 😁.

Si vous changer le système d'exploitation de votre téléphone Android avec un autre Android, imaginons par exemple que vous avez un Samsung et que vous souhaitez installer LineageOS à la place de OneUI, vous pourrez en effet toujours bénéficier des mises à jour d'Android (grâce aux bénévoles de LineageOS) même si Samsung a arrêté le support de votre smartphone. Cependant, le firmware ne pourra jamais être mise à jour, car uniquement Samsung peut le faire ! C'est un énorme risque de sécurité qui ne devrait pas être pris à la légère !

Le firmware, pour expliquer grossièrement, ne fait pas parti du système d'exploitation d'Android. C'est le mini-système d'exploitation des composants intégrés à votre téléphone.

> Si le firmware n'est pas mis à jour, de grosses failles de sécurités peuvent survenir. Un smartphone qui n'est plus supporté par les constructeurs est complètement vulnérable !

C'est pour cela que je vous recommande un Google Pixel. Je vous conseille même de prendre au minimum un Google Pixel 6 (ou 6 pro, ou 6a), car tous les Google Pixel à partir du 6, bénéficieront de [5 ans de mises à jour de sécurité](https://support.google.com/pixelphone/answer/4457705?hl=fr#zippy=%2Ct%C3%A9l%C3%A9phones-pixel-et-versions-ult%C3%A9rieures) minimum !

---

Cependant, je vous **DÉCONSEILLE** d'[installer LineageOS](https://madaidans-insecurities.github.io/android.html#lineageos) sur votre téléphone, car vous devez [déverrouiller le bootloader](https://madaidans-insecurities.github.io/android.html#unlocking-the-bootloader), et cela détruit tout le modèle de sécurité d'Android. Je vous conseille soit de garder l'Android que vous avez par défaut, ou alors d'installer [GrapheneOS](https://grapheneos.org/install/web), car vous pouvez reverrouiller le bootloader.

---

### Bootloader

Pour faire simple, le [bootloader](https://www.reddit.com/r/LineageOS/comments/n7yo7u/a_discussion_about_bootloader_lockingunlocking/) est la partie qui cherche ce qu'il faut démarrer (ici, Android) juste après la mise sous tension de l'appareil. Le bootloader possède une fonctionnalité appelée "[Android Verified Boot](https://privsec.dev/os/choosing-your-android-based-operating-system/#verified-boot)" (AVB) ou "démarrage sécurisé" en français. AVB permet entre autre de vérifier que le système d'exploitation est correct et n'a pas été modifié (par un virus, par quelqu'un ou par autre chose) ! Si le système avait été modifié, AVB aurait annulé ces modifications au démarrage !

Si vous déverrouillez votre bootloader, AVB sera désactivé, et donc vous aurez un manque total de sécurité sur votre smartphone.

Vous ne pouvez pas reverrouiller votre smartphone avec LineageOS, mais vous pouvez cependant le faire avec GrapheneOS ! Ne vous inquiétez pas, l'installation de GrapheneOS est moins compliqué qu'il n'y paraît 😉, et tout fonctionnera pareil que d'habitude (mais en plus sécurisé).

Si vous souhaitez l'installer, vous devez posséder un Google Pixel (quelqu'il soit, de préférence à partir des Pixel 6 pour bénéficier des 5 ans de mises à jour), puis vous devez [suivre les instructions](https://grapheneos.org/install/web) sur leur site web (ne sautez pas d'étapes, suivez les instructions à la lettre, et ça fonctionnera).

### Antivirus

Pour la sécurité de votre smartphone, [n'installez **PAS**](https://privsec.dev/os/android-tips/#manage-android-permissions) d'antivirus, gratuits ou payants. Les antivirus se basent sur le [badness enumeration](https://privsec.dev/knowledge/badness-enumeration/#antiviruses) (littéralement : l'énumération du mal) qui est une méthode complètement détachée de la réalité.

Je vous suggère de lire l'article de Wonderfall concernant la [sécurité sur les smartphones](https://wonderfall.space/modele-securite-mobile/).

### Code PIN

Je vous ***déconseille très fortement*** d'utiliser des [schémas](https://wonderfall.space/password/#le-cas-dun-smartphone) (ou [patterns](https://privsec.dev/os/android-tips/#use-a-diceware-passphrase-avoid-pattern-unlock)) pour déverrouiller votre téléphone. Une [étude](/smartphones/Cracking-Android-Pattern-Lock-in-Five-Attempts.pdf), a prouvé l'inefficacité des schémas. Si vous possédez un Google Pixel ou un iPhone vous pouvez utiliser un code PIN, ces deux téléphones sont tellement sécurisés que juste mettre un code PIN à 4 chiffres prendrait plusieurs dizaines d'années à être [bruteforce](/basiques/password-managers#pourquoi-un-mot-de-passe-doit-comporter-des-majuscules-et-des-caract%C3%A8res-sp%C3%A9ciaux-) (mais mettez quand même 8 chiffres au minimum).

De manière générale, je vous conseille d'utiliser un code PIN à 6 chiffres. Cependant, il serait plus avisé de mettre un code PIN de 8 chiffres ou plus. Et non, ne mettez **pas** la vitesse de la lumière, le nombre pi, ou n'importe quelle autre constante mathématique. Et surtout ne mettez pas votre date de naissance, celle d'un proche ou de votre animal.

Vous pouvez, en complément, utiliser l'empreinte digitale, cela évitera que les gens vous voient taper votre code PIN.

## Le problème des prix

Alors oui la sécurité et la vie privée ont très souvent un prix, je vous conseille donc de prendre la version "a" des Google Pixel, comme le Google Pixel 6a ou le Google Pixel 7a. Il y a beaucoup de réductions en ce moment (la version charbon est actuellement disponible aux alentours de [330€](https://www.amazon.fr/dp/B0B4DN441N/ref=twister_B0BLHRVSSD?_encoding=UTF8&th=1) sur Amazon, faites attention à ce qu'il soit neuf, et non d'occassion, c'est trompeur sur Amazon). Le Google Pixel 7a est actuellement à 509€, si vous souhaitez économiser, je vous conseille d'acheter le 7a dans quelques mois (aux alentours d'octobre ou novembre).

De plus, si vous achetez des smartphones à 200€ tels que les Xiaomi par exemple, vous perdrez plus d'argent, car XIaomi ne possède pas beaucoup de support (2 ans en moyenne) et ils ont une facheuse tendance à ralentir rapidement au fil du temps... Si vous rachetez un smartphone tous les 2 ans, au bout de 5 ans vous aurez payé 500€ (200+200+100). Si vous achetez un Google Pixel 6a au prix fort, 409€ au moment où je vous écris, vous économisez bien 91€ sur 5 ans (car le Google Pixel 6a a 5 ans de mises à jour), voire plus si vous arrivez à avoir des réductions (aux alentours de 330€ en ce moment, donc vous économisez 170€ sur 5 ans).

*Juste pour information, ne tardez pas non plus à acheter votre Google Pixel 6a, car si vous l'achetez après Juillet 2023, vous n'aurez plus que 4 ans de mises à jour, car le support du Pixel 6a s'arrête en [Juillet 2027](https://support.google.com/pixelphone/answer/4457705?hl=fr#zippy=%2Ct%C3%A9l%C3%A9phones-pixel-et-versions-ult%C3%A9rieures). Il sera donc peut-être plus rentable d'acheter le Pixel 7a quand il sortira, mais tout dépend de votre budget.*

Car en effet je vous conseille de garder votre smartphone jusqu'à ce que :

1. Le support s'arrête
2. Il soit tellement cassé qu'il soit inutilisable/irréparable.

Pour conclure, oui 409€ c'est cher, mais étalé sur 5 ans, ça reste abordable. De plus, vous pourrez probablement l'avoir à beaucoup moins cher que ça au moment où vous lirez cet article.

### Notes

J'ai fait ce chapitre sur les prix des smartphones, mais je ne suis pas ici pour vous dire comment dépenser votre argent.

Cependant, j'avais besoin d'écrire un article là-dessus car certaines personnes sous-estiment parfois le prix des smartphones.

Pour vous donnez une fourchette de prix raisonnable pour un smartphone décent, il faut compter entre 300 et 500€. En dessous de 300€, vous trouverez rarement des smartphones qui dureront dans le temps.

Pour les iPhones, je vous conseille de prendre un iPhone SE, ils ont tendance à être moins chers que les hauts de gamme, et restent tout de même très performants. Vous pouvez vous procurer un SE à partir de l'iPhone SE 2020 au minimum (également appelé "2ème génération"), la première génération (2016) possèdant du matériel trop vieux, donc moins sécurisé, le support risque en plus de s'arrêter prochainement puisqu'il est mis à jour depuis déjà 6 ans.

L'iPhone SE 2020 n'étant plus mis en vente, vous pouvez l'acheter d'occasion ou en reconditionné. Amazon propose un service de reconditionnement et vend actuellement l'[iPhone SE 2020 à ~220€](https://www.amazon.fr/Apple-iPhone-G%C3%A9n%C3%A9ration-128GB-Reconditionn%C3%A9/dp/B08D377VBX/ref=sr_1_3?__mk_fr_FR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=24I830FY88X68&keywords=iphone+se+2020&qid=1675455647&sprefix=iphone+se+2020%2Caps%2C110&sr=8-3).

## Fairphone

Je vous déconseille fortement le Fairphone car il [n'est pas sécurisé par défaut](https://privsec.dev/os/android-tips/#phones-to-avoid). En effet, Fairphone met à jour leurs téléphones pendant plusieurs années (leur premier téléphone de 2013 est toujours mise à jour) mais ne met pas à jour les firmwares ! Car seuls les constructeurs Qualcomm peuvent le faire !

Qualcomm est l'entreprise qui créée la plupart des composants tels que les processeurs, puces graphiques, cartes mères pour la plupart des smartphones (Samsung, Xiaomi, OnePlus, Fairphone, etc.). C'est Qualcomm qui, en réalité, met à jour les firmwares de ces composants, les entreprises ne font que suivre ces mises à jour.

> Google construit ses propres composants depuis le Google Pixel 6, c'est pourquoi ils peuvent le mettre à jour pendant 5 ans, voire plus si Google le souhaitait. Même chose pour Apple avec leur propres composants.

De plus, Fairphone utilise souvent les avant-derniers processeurs et autres composants de Qualcomm, sachant que Qualcomm met à jour ses composants pendant environ 3 ans, Fairphone utilise donc des composants qui sont en fin de support. Pour réitérer, quand vous achetez un Fairphone, vous achetez un smartphone qui n'est déjà presque plus supporté par les constructeurs !!! C'est un gros problème de sécurité !

Alors évidemment, je suis pour l'écologie et la protection de l'environnement, mais il faut avoir une bonne balance entre sécurité, vie privée et écologie. Si vous prenez un Xiaomi par exemple, vous n'avez ni sécurité (par rapport à un Google Pixel ou un iPhone), ni respect de votre vie privée, ni respect de l'environnement. En prenant un Fairphone, vous respectez un peu l'environnement (ça reste polluant de fabriquer un smartphone), vous n'avez pas de vie privée (les Services Google Play sont toujours là) et pas de sécurité du tout ! Avec un Google Pixel, vous gagnez en sécurité, et en écologie car vous gardez votre téléphone 5 ans, mais vous ne gagnez toujours pas en vie privée. Cependant, si vous installez GrapheneOS sur votre Pixel, vous gagnez en sécurité, écologie et en vie privée !

## iPhones

J'avoue ne pas être un grand fan d'Apple et je ne connais pas très bien le sujet. Je vous conseille donc de lire l'[article sur IOS par Wonderfall](https://wonderfall.space/modele-securite-mobile/#ios-chez-apple-la-prison-dor-e) qui en parle mieux que moi.

Cela dit, je tiens à prévenir que si Apple promet de respecter votre vie privée, nous n'avons en réalité aucune preuve. Peut-être la respecte-il, peut-être que non, peut-être un peu des deux. Parfois, on voit bien qu'Apple n'a pas accès à certaines données car le chiffrement de bout en bout est implémenté ou que les données restent en local. Cependant ce n'est pas toujours le cas.

iCloud ne propose pas de [chiffrement de bout en bout](/basiques/instant-messengers#le-chiffrement-de-bout-en-bout) pour la [plupart des services](https://support.apple.com/fr-fr/HT202303), tels que vos sauvegardes, vos contacts, vos calendriers, vos photos, etc.

> N'ayez confiance en un service cloud **uniquement** si celui-ci propose du **chiffrement de bout en bout** !

iCloud Backup [sauvegarde votre historique iMessage avec la clé pour pouvoir le déchiffrer](https://support.apple.com/fr-fr/HT202303#messages) (si ce dernier est activé). *(Sachant que les sauvegardes ne sont pas protégées par le chiffrement de bout en bout.)*. Donc oui, **Apple a accès à vos messages** si vous activez **iCloud Backup**.

En ce qui concerne la sécurité, les iPhones sont excellents. En revanche, je ne dis pas que les iPhones sont meilleurs qu'Android sur ce point. Je dirais qu'ils sont plutôt [équivalents](https://www.reddit.com/r/GrapheneOS/comments/bddq5u/comment/ekxifpa/).
Par contre, les iPhones **ET** les Google Pixels sont bien les meilleurs en terme de sécurité que tout le reste du marché des mobiles. Si vous installez GrapheneOS sur un Google Pixel, vous êtes gagnant en sécurité et dans la protection de vos données. Si vous avez un iPhone vous gagnez en sécurité, mais vous êtes un peu perdant concernant vos données.

Tout ceci est mon interprétation de l'[article de Wonderfall](https://wonderfall.space/modele-securite-mobile/#ios-chez-apple-la-prison-dor-e). Je vous invite donc fortement à le lire pour vous faire votre propre opinion.

> Je vous conseille quand même un Google Pixel au lieu d'un iPhone car vous pouvez choisir quelles applications utiliser, vous pouvez prendre Brave ou Firefox au lieu de Safari. Beaucoup d'applications sont bien meilleures sur Android. Sur IOS, vous êtes limité voire bloqué.

---

Sur IOS, tous les navigateurs web [doivent utiliser le même moteur de rendu](/alternatives/apps/#pour-ios), celui d'Apple : WebKit. Donc en utilisant Brave, Google Chrome ou Firefox, c'est comme si vous utilisiez Safari.

---

Depuis [IOS 16.2](https://support.apple.com/en-us/HT213407#162), vous pouvez activer l'option **Advanced Data Protection**, ce qui permet de bénéficier du chiffrement de bout en bout pour des [services essentiels](https://support.apple.com/fr-fr/HT202303#tableWraper) tels qu'iCloud Backup, iCloud Drive, Photos, Notes, Rappels, Signets Safari, Raccourcis Siri, Dictaphones et vos cartes (Wallet).

Je vous recommande fortement de l'[activer](https://support.apple.com/fr-fr/HT212520) pour votre vie privée.

Vous avez besoin de [Raivo OTP](https://raivo-otp.com/) pour le 2FA (Two Factor Authentication), disponible sur l'App Store, cette application sert uniquement pour votre compte Apple. Et vous avez également besoin d'enregistrer la clé de récupération dans votre gestionnaire de mots de passe préféré afin de déchiffrer vos données dans le cas d'une perte de votre téléphone ou d'un changement.

## Conclusion

Pour réitérer :

- Prenez uniquement un Google Pixel (à partir du 6, car 5 ans de support) ou un iPhone récent ([A12+](https://fr.wikipedia.org/wiki/Apple_A12_Bionic)) (à partir de l'iPhone XR/XS/XS Max).
- N'installez **pas** d'applications qui se disent améliorer la sécurité ou la performance de votre téléphone. Suivez la [règle KISS](https://fr.wikipedia.org/wiki/Principe_KISS).
- Utilisez un code PIN de 6 chiffres minimum, mais 8 chiffres ou plus est recommandé.
- Installez GrapheneOS sur votre Google Pixel.
- Achetez uniquement des téléphones neufs ou quasi-neufs. N'achetez pas de téléphones qui ne sont plus supportés.
- Si vous avez acheté un autre téléphone, revendez-le (surtout si c'est un Fairphone) et achetez un Google Pixel 6/6a/6 Pro (ou un iPhone).
- Si vous avez acheté des antivirus (ou d'autres applications comme CCleaner), arrêtez ces abonnements, car vous jetez littéralement de l'argent par les fenêtres. Puis achetez un smartphone récent grâce aux économies que vous aurez faites. (Car il est plus sécurisé d'utiliser un smartphone récent et mis à jour régulièrement qu'un vieux téléphone doté d'un antivirus.)

---

## En savoir plus & crédits

- [Le modèle de sécurité mobile - Wonderfall](https://wonderfall.space/modele-securite-mobile/)
- [Android - Madaidan](https://madaidans-insecurities.github.io/android.html) (en anglais)
- [Android Tips - PrivSec.dev](https://privsec.dev/posts/android/android-tips/) *(site en anglais, j'ai le même thème que son site web car c'est un thème publique et gratuit, ne soyez pas étonné)*
- [Badness Enumeration - PrivSec.dev](https://privsec.dev/posts/knowledge/badness-enumeration/) (en anglais)
