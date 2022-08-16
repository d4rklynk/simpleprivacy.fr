---
title: "Les bonnes pratiques sur Internet 👍️"
date: 2022-08-16
weight: 1
---

Ce guide va vous permettre d'adopter des bonnes pratiques pour regagner votre vie privée mais également pour gagner en sécurité ! Tout ça sans trop d'efforts !

Ce sera une liste brute et rapide de ce que vous devez faire ou non. Si vous souhaitez plus d'infos, je vous enverrai vers mes autres articles ou vers des liens externes.

## Sécurité
### Sécurité sur votre PC et votre smartphone

- [N'installez pas d'antivirus](/basiques/threat-model/#se-protéger-des-virus-et-des-hackers), Windows Defender suffit amplement. Et je vous **déconseille** d'installer des [antivirus sur votre smartphone](/basiques/smartphones/#antivirus).
- N'installez pas d'applications qui se disent améliorer les performances (donc n'installez pas des applications comme CCleaner).
- [KISS](https://fr.wikipedia.org/wiki/Principe_KISS). Installez le minimum.
- Créez une [phrase de passe robuste](/basiques/password-managers/#la-méthode-diceware) pour vos sessions sur vos PC.
- [Créez un code PIN](/basiques/smartphones/#code-pin) **aléatoire**, et j'insiste sur l'**aléatoire**, d'au moins 8 chiffres sur votre smartphone. Vous pouvez utiliser l'empreinte difitale en complément.
- Ne branchez jamais une clé USB que vous ne connaissez pas. Si vous en trouvez une par terre, détruisez-la et jetez-la.
- Évitez un maximum de prêter votre PC ou votre smartphone. Si cependant vous êtes amené à le faire, créez une autre session sur Windows. Vous pouvez aussi créer un autre profil sur Android.
- Vérifiez les permissions de vos applications sur Android/IOS et désactivez tout ce qui est inutile. Est-ce qu'Instagram ou TikTok a besoin de connaître votre agenda ou vos contacts par exemple ?
- N'achetez pas de smartphones qui sont en [fin de support](/basiques/smartphones/#aosp-et-firmware).
- **Mettez à jour vos appareils.**
- Chiffrez les disques de vos PC.
- Faites toujours le raccourci **WIN + L** quand vous quittez (même 10 secondes) votre PC, ne le laissez jamais ouvert.

### Sécurité sur Internet

- Utilisez un [gestionnaire de mots de passe](/basiques/password-managers). Sérieusement, faites-le. [Bitwarden](/fiches/bitwarden) est excellent.
- Utilisez des mots de passe à **20 caractères au grand minimum !**
- Partez du principe que chaque site web n'est pas digne de confiance. C'est bien de vérifier que le cadenas est présent sur l'URL mais ce cadenas ***prouve uniquement que le site est chiffré***, rien ne garantit l'[authenticité](/basiques/instant-messengers/#la-signature-digitale) du site ! Ce qui veut dire que le site a beau être chiffré, c'est peut-être un faux site pour récupérer vos identifiants.
- Activez le ***mode HTTPS uniquement*** sur votre navigateur.
- Partez du principe que chaque SMS est frauduleux, la sécurité des SMS est complétement dépassée. Évitez un maximum d'utiliser les SMS et utilisez [Signal](/basiques/instant-messengers/#signal) à la place.
- Évitez un maximum les mails, si vous devez quand même les utiliser, choisissez [Proton Mail](https://proton.me/fr). Partez du principe que chaque mail est peut-être une arnaque. Ne cliquez jamais sur les liens présents dans les mails, ouvrez un nouvel onglet et allez directement sur le site correspondant au lien. 

> Exemple : Vous recevez un mail car vous avez un problème avec votre compte bancaire. **Allez sur un nouvel onglet**, allez sur votre banque, vérfiez que vous n'avez pas de messages dans votre application de banque. Si vous avez un doute, appelez votre banque.

> Autre exemple : Vous recevez un mail comme quoi vous avez été piraté, il vous montre même votre **mot de passe**, parce que Monsieur est super fort ! Vous devez le payer en cryptomonnaies ou sinon il dilvuguera tout sur Internet ! **Supprimez le mail, c'est totalement bidon. Pour l'explication, si il y a eu une fuite de données sur un site web, vos mots de passe et vos mails sont dans la nature. Des arnaqueurs prennent ensuite le mot de passe et l'envoient au mail correspondant, ils le font avec un programme pour envoyer ces mails en masse. Donc dans votre mail, oui le mot de passe est bien le vôtre, mais non ils n'ont aucune donnée.**

- Ne donnez vos mots de passe à **personne**, **sous aucun prétexte**.
- Utilisez la double authentification sur tous les sites où vous pouvez le faire. Utiliez l'application **Aegis**.
- Mettez un mot de passe Wifi robuste et utilisez WPA2 au minimum. N'utilisez pas WEP, il prend trois minutes à cracker (je l'ai fais).

## Vie privée

- **[Mentez](/basiques/threat-model/#protéger-votre-vie-privée-du-capitalisme-de-la-surveillance)**. On n'a pas besoin de savoir qui vous êtes, mettez le minimum d'informations, et mentez sur votre âge, votre sexe, votre statut marital, etc.
- Utilisez [Signal](/basiques/instant-messengers/#signal).
- Gardez vos données pour vous, évitez un maximum de les mettre en ligne (le fait de partagez vos photos sur [Facebook Messenger](/basiques/instant-messengers/#facebook-messenger) est équivalent à les mettre en ligne), si vous le devez, utilisez un service proposant du [chiffrement de bout en bout](/basiques/instant-messengers/#le-chiffrement-de-bout-en-bout). 

> Ma définition de mettre en ligne un fichier : c'est à partir du moment où la donnée sort de votre PC ou de votre smartphone.