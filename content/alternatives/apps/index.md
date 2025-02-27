---
title: "Les applications \U0001f4da"
date: 2022-08-03
---
## Les navigateurs web sur PC

Si vous utilisez Google Chrome, Opera, Vivaldi ou tout autre navigateur, changez pour un autre navigateur plus respectueux de votre vie privée.

- [Brave](https://brave.com/fr/)
- [Mullvad](https://mullvad.net/fr/browser)

    > Mullvad fonctionne comme Tor Browser (mais sans le réseau Tor), il est important d'utiliser Mullvad Browser avec un VPN. Sinon, utilisez Brave ou Firefox. Pour le choix d'un VPN, vous pouvez voir les alternatives que je propose [ici](/alternatives/providers/#les-vpns).

- [Firefox](https://www.mozilla.org/fr/firefox/new/) (mais préférez Brave)

---

## Les navigateurs web sur smartphone

Les recommendations ne sont pas les mêmes que sur PC pour des raisons de sécurité. Pour l'instant Firefox n'est pas conseillé sur Android ou IOS.

### Pour Android

- Brave
- (Vanadium si vous utilisez GrapheneOS)

> Firefox manque actuellement de certaines [mesures de sécurité](https://madaidans-insecurities.github.io/firefox-chromium.htm).

### Pour IOS

- Uniquement Safari

> Il faut comprendre que les navigateurs web ont un cœur appelé "moteur de rendu", c'est ce cœur qui permet au navigateur d'afficher les pages web. Firefox utilise le moteur de rendu **Gecko** et tous les navigateurs basés sur Chromium (Google Chrome, Brave, Vivaldi, Opera, Samsung Internet, Microsoft Edge) utilisent **Blink**. Sur IOS, Safari utilise **WebKit**, et tous les navigateurs pour IOS sont obligés d'utiliser ce moteur de rendu (WebKit). Donc, en utilisant Firefox ou Brave, vous "n'échappez" pas à l'écosystème d'Apple, et Apple peut donc voir tout ce que vous faites sur Firefox (et tout autre navigateur sur IOS) autant que sur Safari. En utilisant Safari, vous réduisez votre confiance à une seule entité : Apple. Alors qu'en utilisant Firefox ou un autre navigateur sur IOS, vous faites confiance à Apple **et** à un autre organisme. C'est mieux de faire confiance à une seule entité qu'à plusieurs.

---

## Les applications de prise de notes

Si vous utilisez Google Keep, ou OneNote, pensez à choisir une autre application.

Je vous conseille uniquement des applications qui implémentent le chiffrement de bout en bout.

- [Joplin](https://joplinapp.org/)

    > Vos notes sont par défaut enregistrées en local, vous pouvez cependant synchroniser vos notes via OneDrive (Microsoft), mais le chiffrement de bout en bout n'est pas actif par défaut ! Vous devez l'activer dans les paramètres de Joplin ! Activez le chiffrement de bout en bout **AVANT** de synchroniser avec OneDrive.

- [Standard Notes](https://standardnotes.com/)

---

## Partage de fichiers

De manière générale, je vous recommande d'utiliser le plus possible Signal ou WhatsApp pour le partage de fichiers (car elles implémentent du chiffrement de bout en bout par défaut). Si vous ne pouvez pas, ou que les fichiers sont trop gros, je vous conseille d'aller sur [hat.sh](https://hat.sh/), de chiffrer le fichier désiré avec un mot de passe et de le partager sur votre plateforme de partage de fichiers préféré. Ainsi uniquement vous et le destinataire auront accès au fichier (vous donnez le mot de passe du fichier par Signal ou WhatsApp évidemment, et surtout pas par SMS ou par mail).

***N'utilisez pas le mail ou les SMS pour partager vos fichiers.***

Ces deux projets implémentent le chiffrement de bout en bout. Vous pouvez donc partagez vos fichiers sereinement.

Protégez ***toujours*** vos partages avec un mot de passe !

- [Syncthing](https://syncthing.net/)
- Bitwarden Send (uniquement version Premium), jusqu'à 1 Go.
- [Send](https://send.vis.ee/)

    > Send est un fork de Firefox Send. Firefox ayant arrêté le projet, des volontaires ont continué leur propre truc basé sur ce projet. Je précise que Send est basé sur le projet de Firefox Send, mais ce **N'EST PAS** Firefox, ce sont des volontaires. Plusieurs [instances](https://github.com/timvisee/send-instances/) sont disponibles (stockage différent ou délai d'expiration différents). Une instance est un serveur d'un volontaire qui héberge le programme Send.

---

## Les gestionnaires de mots de passe

Je vous conseille fortement [Proton Pass](https://proton.me/fr/pass) ou [Bitwarden](https://bitwarden.com/).

---

## Les applications de 2FA

Le 2FA ("Two Factor Authentication" ou "Double Authentification" en français) est essentiel pour votre sécurité en ligne. Si quelqu'un a accès à votre identifiant de compte et votre mot de passe, il ne pourra toujours pas s'y connecter sans le code OTP (One-Time Password), un code à 6 chiffres qui change en général toutes les 60 secondes.

- [Aegis](https://getaegis.app/) - [Play Store](https://play.google.com/store/apps/details?id=com.beemdevelopment.aegis)
- [Ente Auth](https://ente.io/auth/) - [Play Store](https://play.google.com/store/apps/details?id=io.ente.auth)

> N'oubliez pas de faire des sauvegardes d'Aegis (vous pourrez exporter les codes OTP en naviguant dans les paramètres d'Aegis) ! Vous pouvez ensuite les téléverser (ou *upload* en anglais) dans un service cloud chiffré de bout en bout tel que Proton Drive ou sur un disque chiffré en local chez vous.

---

## Les applications de productivité

Si vous possédez déjà Microsoft Office, je vous conseille de l'utiliser (simplement car il est bien plus sécurisé que toutes les alternatives proposés ici). Si vous ne possédez pas Microsoft Office et que vous n'avez pas le budget (voir [les prix](https://www.microsoft.com/fr-fr/microsoft-365/p/microsoft-365-personnel/cfq7ttc0k5bf) sur le site Microsoft) je vous conseille ces solutions :

- [OnlyOffice](https://www.onlyoffice.com/en/download-desktop.aspx)

    > OnlyOffice est de loin la meilleure alternative, elle ressemble fortement à Microsoft Office, et est donc simple à utiliser pour ceux qui adorent l'interface de Microsoft Office. Les fichiers venant de la suite Microsoft ne sont rarement, voire jamais cassés quand ils sont importés sur OnlyOffice.

- [CryptPad](https://cryptpad.fr/)

    > CryptPad est une suite logicielle basée sur le web, de la même manière que **G Suite** (ou **Google Workspace**) qui est uniquement disponible via le navigateur. CryptPad est chiffré de bout en bout, vous pouvez créer et partager un fichier (Word, Excel, PowerPoint, etc) sans compte. Mais vous pouvez tout de même créer un compte et accéder à quelques fonctionnalités supplémentaires. Des [options payantes)(https://cryptpad.fr/features.html) sont disponibles.

---

## Les messageries instantanées

J'ai écris un article sur les [messageries instantanées](/basiques/instant-messengers/).

Je vous conseille d'utiliser uniquement Signal et de convaincre votre entourage de l'utiliser également. Signal est riche en fonctionnalités, est très joli, et implémente par défaut le chiffrement de bout en bout. C'est la messagerie la plus sécurisée qu'on puisse avoir aujourd'hui.

- [Signal](https://www.signal.org/fr/)

    > Si vous n'avez pas réussi à convaincre une partie de votre entourage, je vous conseille, de réessayer de les convaincre. Si ce n'est pas possible, alors utilisez WhatsApp plutôt que Facebook Messenger. WhatsApp implémente le chiffrement de bout en bout par défaut contrairement à Facebook Messenger où c'est optionnel ! Cependant, WhatsApp collecte énormément vos [métadonnées](/basiques/instant-messengers/#métadonnées).

- [SimpleX Chat](https://simplex.chat/)

    > SimpleX Chat vous propose de communiquer avec les autres sans identifiants, c'est à dire que votre compte n'existe ni grâce à un numéro de téléphone, ni par un mail, ni par un nombre aléatoire. Je vous laisse découvrir ça sur leur [site web](https://simplex.chat/#simplex-explained). L'application est disponible sur [IOS](https://apps.apple.com/us/app/simplex-chat/id1605771084) et sur [Android](https://play.google.com/store/apps/details?id=chat.simplex.app). La création du compte est local (vous donnez uniquement un pseudonyme), si vous supprimez l'application, vous n'y aurez plus accès (sauf si vous exportez/importez vos messages).

## Alternatives à YouTube

NewPipe ou LibreTube sur Android sont recommandés. Toutes les pubs dans les vidéos sont enlevées. Toutes les vidéos proviennent de YouTube, ces applications ne sont pas développées par Google mais par des bénévoles.

- [NewPipe](https://newpipe.net/)
- [LibreTube](https://libretube.dev/)
