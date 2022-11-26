---
title: "Les bonnes pratiques sur Internet 👍️"
date: 2022-08-16
weight: 1
---

![Bonnes pratiques cover](/bonnes-pratiques/bonnes-pratiques-cover.jpg)

Ce guide va vous permettre d'adopter des bonnes pratiques pour regagner votre vie privée mais également en sécurité ! Tout ça sans trop d'efforts !

Ce sera une liste brute et rapide de ce que vous devez faire ou non. Si vous souhaitez plus d'infos, je vous enverrai vers mes autres articles ou vers des liens externes.

## Sécurité
### Sécurité sur votre PC et votre smartphone

- Pour les smartphones, achetez un Google Pixel (à partir du 6 si vous souhaitez bénéficier de 5 ans de support). J'explique pourquoi dans mon [article sur les smartphones](/basiques/smartphones/#recommandations).
- Utilisez macOS, ChromeOS ou Windows 11 pour les PC.
- [N'installez pas d'antivirus](/basiques/threat-model/#se-protéger-des-virus-et-des-hackers), Windows Defender suffit amplement. Et je vous **déconseille** d'installer des [antivirus sur votre smartphone](/basiques/smartphones/#antivirus).
- N'installez pas d'applications qui se disent améliorer les performances (donc n'installez pas des applications comme CCleaner).
- [KISS](https://fr.wikipedia.org/wiki/Principe_KISS). Installez le minimum.
- Créez une [phrase de passe robuste](/basiques/password-managers/#la-méthode-diceware) pour vos sessions sur vos PC.
- [Créez un code PIN](/basiques/smartphones/#code-pin) **aléatoire**, et j'insiste sur l'**aléatoire**, d'au moins 8 chiffres sur votre smartphone. Vous pouvez utiliser l'empreinte digitale en complément.
- Ne branchez jamais une clé USB que vous ne connaissez pas. Si vous en trouvez une par terre, détruisez-la et jetez-la.
- Évitez un maximum de prêter votre PC ou votre smartphone. Si cependant vous êtes amené à le faire, créez une autre session sur Windows. Vous pouvez aussi créer un autre profil sur Android.
- Vérifiez les permissions de vos applications sur Android/IOS et désactivez tout ce qui est inutile. Est-ce qu'Instagram et Facebook ont besoin de connaître votre agenda ou vos contacts par exemple ?
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

> Exemple 1 : Vous recevez un mail car vous avez un problème avec votre compte bancaire. **Allez sur un nouvel onglet**, allez sur votre banque, vérfiez que vous n'avez pas de messages dans votre application de banque. Si vous avez un doute, appelez votre banque.

> Exemple 2 : Vous recevez un mail comme quoi vous avez été piraté, il vous montre même votre **mot de passe** afin que vous y croyez vraiment et vous devez le payer en cryptomonnaies ou il dilvuguera tout sur Internet ! **Supprimez le mail, c'est totalement bidon. Pour l'explication, si il y a eu une fuite de données sur un site web dont vous possédez un compte, vos mots de passe et vos mails se retrouvent en clair dans des listes appelées "wordlist" où se trouvent également les identifiants de plein d'autres gens. Des arnaqueurs prennent ensuite ces paires d'identifiants (mot de passe et mails) et l'envoient au mail correspondant, ils le font avec un programme pour envoyer ces mails en masse. Donc dans le mail, oui le mot de passe est bien le vôtre, mais non, ils n'ont aucune donnée. Changez le mot de passe de votre compte.**

> Exemple 3 : Vous recevez un mail dans lequel on vous informe que votre souscription à Orange va bientôt se finir pour une quelconque raison. Certains vont se dire "Je vais pas me faire avoir, je suis chez SFR moi !". En réalité ce genre de mails sont envoyés en masse, le but est de se baser sur les coïncidences dans votre vie. Donc certains ne tomberont pas dans le panneau, car il ne sont pas chez Orange, mais d'autres le sont, et ce sont eux qui risquent de se faire le plus avoir. 

> Le principe du phishing (ou hammeçonnage en français) repose sur le fait qu'un poisson parmi d'autres va mordre. Une majorité se doutera que le mail est frauduleux, mais une petite partie se fera tout de même avoir. (Je vous rassure, n'ayez pas honte si cela vous arrive, certains phishing sont très bien fait, mais faites passer le mot pour que personne ne puisse se faire avoir comme vous.)

- Ne donnez vos mots de passe à **personne**, **sous aucun prétexte**.
- Utilisez la double authentification sur tous les sites où vous pouvez le faire. Utilisez l'application **[Aegis](https://getaegis.app/)**.
- Mettez un mot de passe Wifi robuste et utilisez WPA2 au minimum. N'utilisez pas WEP, il prend trois minutes à cracker (je l'ai fait).

## Vie privée

- **[Mentez](/basiques/threat-model/#protéger-votre-vie-privée-du-capitalisme-de-la-surveillance)**. On n'a pas besoin de savoir qui vous êtes, mettez le minimum d'informations, et mentez sur votre âge, votre sexe, votre statut marital, etc.
- Utilisez [Signal](/basiques/instant-messengers/#signal).
- Gardez vos données pour vous, évitez un maximum de les mettre en ligne (le fait de partagez vos photos sur [Facebook Messenger](/basiques/instant-messengers/#facebook-messenger) est équivalent à les mettre en ligne), si vous le devez, utilisez un service proposant du [chiffrement de bout en bout](/basiques/instant-messengers/#le-chiffrement-de-bout-en-bout). 

> Ma définition de mettre en ligne un fichier : c'est à partir du moment où la donnée sort de votre PC ou de votre smartphone.

- N'installez pas un paquet d'extensions d'anti-tracking sur votre navigateur, c'est inutile, et cela va même vous rendre encore plus facilement pistable. [uBlock Origin](https://ublockorigin.com/) suffit largement sur Firefox. Brave inclut déjà par défaut quelque chose de similaire à Ublock Origin (nommé [Brave Shield](https://brave.com/shields/)), c'est donc inutile de l'installer sur ce dernier.
- Évitez de créer des comptes dans tous les sens. Demandez-vous si vous en avez vraiment besoin (**SPOILER** : la réponse est souvent non). Rappelez-vous que c'est toujours très facile de créer un compte en ligne, mais c'est toujours très compliqué voire impossible de le supprimer.

---

En savoir plus & crédits

- [Security and Privacy Advice - Madaidan](https://madaidans-insecurities.github.io/security-privacy-advice.html)
- [10 dumbest ideas in privacy communities - rhbik5](https://www.reddit.com/r/PrivacyGuides/comments/rhbik5/10_dumbest_ideas_in_privacy_communities/)
