---
title: "Présentation et utilisation de Signal 💬"
date: 2022-08-09
weight: 4
---

![signal cover](signal-cover.png#center)

Aujourd'hui, je vais vous présenter Signal et ses fonctionnalités de base.

Je vous conseille de lire mon article sur les [messageries instantanées](/basiques/instant-messengers) dont un chapitre est dédié à [Signal](/basiques/instant-messengers#signal).

Toutes les [informations concernant l'utilisation de Signal](https://support.signal.org/hc/fr) sont disponibles sur leur site web.

## Installation

Signal peut être installé sur Android, IOS, Windows, Linux et MacOS.

Vous pouvez le télécharger via le Play Store, l'AppStore ou via [leur site](https://signal.org/download/).

## Création du compte

![signal image](signal-intro.png#center)

Vous cliquez sur "**Poursuivre**" puis une fenêtre va s'ouvrir pour demander l'autorisation des contacts.

![signal-contact-autorisation.png](signal-contact-autorisation.png#center)

En acceptant, Signal va pouvoir identifier, [grâce aux numéros de téléphone](https://signal.org/blog/private-contact-discovery/), les contacts qui possèdent déjà Signal. Si vous refusez, vous devrez manuellement ajouter le numéro de téléphone de vos destinataires. Pour des raisons de commodité, je vous conseille de l'activer, mais vous n'êtes pas obligé. Vos contacts sont [stockés localement sur votre téléphone](https://support.signal.org/hc/fr/articles/360007061452-Signal-envoie-t-elle-mon-num%C3%A9ro-%C3%A0-mes-contacts-), donc vous n'avez rien à craindre.

Vous devrez ensuite mettre votre numéro de téléphone.

![signal-signup.png](signal-signup.png#center)

Confirmez le code reçu par SMS, validez le captcha et vous arriverez sur cette page :

![signal-pin-creation.png](signal-pin-creation.png#center)

Je vous suggère ***fortement*** de "**Créer un NIP alphanumérique**" et de [créer une phrase de passe avec la méthode diceware](/basiques/password-managers#la-méthode-diceware), puis, enregistrez-le dans votre [gestionnaire de mots de passe](/basiques/password-managers).

> Le **code NIP** (ou PIN en anglais) vous permet de [récupérer votre profil, vos paramètres, vos contacts et les personnes que vous avez bloqués](https://support.signal.org/hc/fr/articles/360007059792-NIP-Signal) dans le cas où vous auriez perdu ou changé votre téléphone.

Une fois le code NIP enregistré dans votre gestionnaire de mots de passe, vous arriverez sur la page de la création de votre profil :

![signal-profil-creation.png](signal-profil-creation.png#center)

Le prénom est requis, vous pouvez cependant juste écrire un pseudo, un caractère ou même un emoji.

Le [profil](https://support.signal.org/hc/fr/articles/360007459591-Les-profils-Signal-et-les-demandes-d-%C3%A9change-de-messages) est constitué d'un **nom** et d'une **image de profil**. L'image de profil est cependant facultative.

Une fois votre profil rempli, vous arriverez sur la page principale d'accueil de Signal. Félicitations ! Vous êtes sur Signal !

## Conversation

Voici la page d'accueil une fois votre compte créé.

![signal-main-page.png](signal-main-page.png#center)

Si vous souhaitez parler à un de vos contacts (et si vous avez autorisé l'accès au contacts de votre téléphone), attendez quelques minutes le temps que Signal identifie qui de vos contacts possède l'application. Sinon appuyez sur le bouton avec le **crayon** et tapez le numéro de téléphone de la personne que vous souhaitez contacter.

Si la personne n'est pas dans les contacts de votre téléphone (ou que vous n'avez pas autorisé l'accès aux contacts), vous devrez attendre que la [personne accepte la demande de contact](https://support.signal.org/hc/fr/articles/360007459591-Les-profils-Signal-et-les-demandes-d-%C3%A9change-de-messages#message_requests).

![signal-new-message.png](signal-new-message.png#center)

Vous arriverez ensuite sur la conversation du contact que vous avez ajouté. Vous pouvez commencer à converser.

![signal-salut.png](signal-salut.png#center)

Les petites icônes en bas à droite sont expliquées dans la [documentation de Signal](https://support.signal.org/hc/fr/articles/360007320751-Comment-puis-je-savoir-si-mon-message-a-%C3%A9t%C3%A9-remis-ou-lu-).

## Paramètres

Vous avez deux types de paramètres :

- [Les paramètres généraux](#les-paramètres-généraux)
- [Les paramètres de conversation](#les-paramètres-de-conversation)

### Les paramètres généraux

Vous pouvez accéder aux paramètres généraux en cliquant sur votre **profil en haut à gauche** sur la **page d'accueil** de Signal.

![signal-settings.png](signal-settings.png#center)

C'est ici que vous pourrez changer l’apparence de Signal (en mode sombre par exemple) ou la couleur des conversations par défaut.
Vous pouvez changer votre code NIP dans "**Compte**" si jamais vous l'avez oublié.

### Les paramètres de conversation

Les paramètres de conversation sont uniques pour chaque contact. Vous pouvez y accéder en cliquant sur les trois petits points en haut à droite d'une conversation.

![signal-conversation-dots.png](signal-conversation-dots.png#center)

![signal-conversation-settings.png](signal-conversation-settings.png#center)

C'est ici que vous pourrez changer les paramètres par défaut pour ***cette*** conversation uniquement. Vous pouvez activer un délai d'expiration des messages par défaut, changer les couleurs de la conversation, etc.

## Configuration recommandée

### Compte

Je vous suggère d'aller dans les **paramètres généraux** puis dans "**Compte**" et d'activer :

- [x] "Blocage de l'inscription"

![signal-account.png](signal-account.png#center)

[Cela évitera que quelqu'un réinscrive votre numéro de téléphone](https://support.signal.org/hc/fr/articles/360007059792-NIP-Signal#manage_registration_lock). Il aura besoin de votre code NIP.

### Confidentialité

Naviguez dans les **paramètres généraux** puis dans "**Confidentialité**". Activez tous les paramètres dans la section "**Sécurité de l'appli**" :

- [x] Verrou d'écran (puis choisissez 10 minutes environ)
- [x] Sécurité de l'écran (cela évitera les captures d'écran)
- [x] Clavier incognito

![signal-privacy-2.png](signal-privacy-2.png#center)

## SMS/MMS

Optionnellement, vous pouvez utiliser Signal pour envoyer et recevoir des SMS/MMS, cependant ceux-ci ne seront pas chiffrés puisqu'ils n'utiliseront pas les services de Signal. Pour éviter la confusion, je vous conseille d'utiliser une application à part pour les SMS/MMS.

## Fonctionnalités

Je ne vais pas vous faire la liste entière, mais je vais vous lister quelques fonctionnalités importantes. Cette liste est complètement subjective :

- [Note à mon intention](https://support.signal.org/hc/fr/articles/360043272451-Note-%C3%A0-mon-intention)

> Cela permet d'envoyer des messages à vous-mêmes, très pratique pour s'envoyer une note entre son téléphone et son PC si vous avez installé Signal sur votre ordinateur.

- [Autocollants](https://support.signal.org/hc/fr/articles/360031836512-Autocollants) (souvent appelés **stickers**)

> Vous pouvez télécharger des stickers à partir du site non-officiel [Signal Stickers](https://signalstickers.com/). Naviguez sur votre navigateur de votre téléphone, puis cliquez sur "**Add to Signal**". Pour ma part, je vous [conseille](https://signalstickers.com/pack/2a4c8da668bb83cdf1ca2c2e6b0e4f60) [ces](https://signalstickers.com/pack/7b82302290ab9bb92cb66b8b67006df3) [six](https://signalstickers.com/pack/1917d7d33777f7c852d8970321d78f4a) [packs](https://signalstickers.com/pack/486e174c7972aef953f7c9579604ca17) [de](https://signalstickers.com/pack/20d2d82c1de0924634176f139f80f5b7) [stickers](https://signalstickers.com/pack/22cc15c9671421a307aa4da6a76f4249) que j'aime beaucoup.

- Modifier une image

> Lors de l'envoi d'une photo ou d'une image, vous pouvez dessiner, ajouter des stickers ou du texte sur ces médias. Vous pouvez également choisir de l'envoyer en basse ou haute qualité.

Une [liste complète des fonctionnalités](https://support.signal.org/hc/fr/categories/360000674791-Fonctions) de Signal est disponible sur leur site web.
