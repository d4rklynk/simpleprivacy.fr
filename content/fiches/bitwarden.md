---
title: "Bitwarden : Comment l'utiliser \U0001f511"
date: 2022-07-29
weight: 1
---

![Bitwarden](/bitwarden/apps-combo-logo.png)

[Bitwarden](https://bitwarden.com/) est un gestionnaire de mots de passe open source, gratuit et facile.

*J'ai écris un article sur les [gestionnaires de mots de passe](/basiques/password-managers) si vous voulez en savoir plus.*

Aujourd'hui, je vous explique comment l'utiliser.

## Création de votre compte

Allez sur le site de [Bitwarden](https://bitwarden.com/) et cliquez sur le bouton **Get Started** :

![Bitwarden Get Started image](/bitwarden/bitwarden-get-started-header.jpg)

Vous arriverez sur cette page où vous créerez votre compte :

![Signup page image](/bitwarden/bitwarden-signup-page.svg)

Remplissez les cases comme montré ci-dessus et cliquez sur le bouton **Submit**, ce qui aura pourra effet de vous envoyer à la **page de connexion** de Bitwarden comme ci-dessous :

![Bitwarden Login page image](/bitwarden/bitwarden-login-page.png)

Vous entrez vos identifiants et tada !

![Bitwarden Interface image](/bitwarden/bitwarden-interface.png)

Bitwarden est en anglais pour moi, mais ne vous inquiétez pas, ça devrait être affiché en français pour vous !

## L'interface

L'interface de bitwarden n'est pas très compliquée, mais je vais vous montrer comment [ajouter vos mots de passe](#ajouter-lextension-à-votre-navigateur) sur l'extension du navigateur juste après ! Ici je vous présente juste l'interface web, mais vous n'y serez pas souvent.

![Bitwarden Interface Legende](/bitwarden/bitwarden-interface-legend.png)

**En rouge :**

1. C'est la page d'accueil de vos mots de passe, de vos notes sécurisés et de vos cartes bancaires, c'est ici que vous verrez absolument tout.
2. C'est la même chose que la page d'accueil en fait.
3. Si vous supprimez des identifiants, ils finiront à la poubelle.  C'est supprimé automatiquement au bout de 30 jours !
4. - Login : Vos identifiants de connexions
	- Card : Vos cartes bancaires
	- Identity : Vos cartes d'idendités
	- Secure Note : Vos notes sécurisés (très utile pour juste noter des code PIN, comme ceux des cartes bancaires, ou des cartes de magasins !)
5. Ce sont les dossiers que vous créez pour organiser vos mots de passe, mais honnêtement c'est là pour faire joli, c'est vraiment optionnel pour le coup.

**En vert :**

6. - Vault : Votre coffre, là où vous êtes actuellement
	- Send : si vous souhaitez envoyer des fichiers (max : 1Go) à des amis (uniquement avec la version Premium, c'est 10€/an)
	- Tools : C'est ici que vous trouverez notamment le générateur de mots de passe
	- Reports : Ce sont des options premium (c'est pas essentiel, ne vous inquiétez pas)
7. Add item : Vous cliquez dessus pour ajouter vos identifiants 
8. Ce sont vos paramètres de compte

## Importez/Exportez vos mots de passe

*Cette étape est utile pour ceux qui possédent un autre gestionnaire de mots de passe et souhaitent changer pour Bitwarden, vous pouvez exportez vos mots de passe de votre gestionnaire actuel pour l'importer sur Bitwarden.*

L'avantage avec les gestionnaires de mots de passe, c'est que si vous souhaitez changer, ca prend à peine 5 minutes !
Vous exportez vos mots de passe, vous les importez dans le nouveau, vous supprimez votre compte de votre ancien gestionnaire de mots de passe et c'est réglé !

![Bitwarden import data image](/bitwarden/bitwarden-import-data.png)

Vous choisissez dans le menu déroulant de quel gestionnaire de mots de passe vous souhaitez importer vos données, vous cliquez sur **Browse** et choisissez le fichier importé.

Pour exporter vos mots de passe, allez dans **Export Vault**, le processus est tout aussi simple.

## Ajouter l'extension à votre navigateur

***C'est ici qu'on va ajouter vos mots de passe !***

Allez sur sur la [page de téléchargement](https://bitwarden.com/download/) de Bitwarden et cliquez le navigateur sur lequel vous êtes actuellement, puis installez l'extension.

![Bitwarden download page](/bitwarden/bitwarden-download-web-browser.png)

Connectez-vous sur l'extension :

![Bitwarden addon login](/bitwarden/bitwarden-addon-login.png)

On va pouvoir ajouter vos identifiants en appuyant sur "**+**" tout en haut à droite :

![Bitwarden addon](/bitwarden/bitwarden-add-login.png)

Vous arrivez là-dessus :

![Bitwarden adding](/bitwarden/bitwarden-adding.png)

1. Choisissez le type (identifiants, carte bancaire, carte d'identité ou note sécurisée). Vous laissez **"login"** si vous souhaitez ajouter des identifiants de connexion.
2. Le nom de votre identifiant (exemple : "`Pôle Emploi`" ou  "`Google compte du boulot`"), c'est juste le titre, mettez ce qui vous parle le plus (par défault Bitwarden mais le nom domaine, comme "`accounts.google.com`" par exemple).
3. Votre mail/pseudo (ça dépend des sites)
4. Votre mot de passe
5. Ici vous mettez l'URL, au format `https://account.proton.me` par exemple. C'est ce qui permettra de savoir si vous avez des identifiants correspondant pour le site web que vous visitez.

![Number Bitwarden](/bitwarden/bitwarden-number.png)

> Vous pouvez voir que je suis actuellement sur un site web, et Bitwarden a reconnu grâce à l'URL `https://account.proton.me` que j'avais un identifiant correspondant. Si vous avez `2` affiché au lieu de `1` c'est que vous avez deux comptes sur ce site, tout simplement. Au-delà de l'aspect pratique de la chose, elle a aussi un aspect de sécurité, car si vous naviguer sur un site bidon comme `https://account.google.com` (la vrai page de connexion de Google comporte un `s` à la fin de `account`), Bitwarden ne reconnaîtra pas la page et donc n'affichera pas de numéro, ça évite de mettre vos mots de passe sur des sites non-légitimes. Ou alors, vous avez tout simplement oublié d'ajouter l'URL.
 
Le champ de l'URL est automatiquement rempli avec l'URL de la page que vous visitez au moment où vous cliquez sur **"+"**.

*Exemple : Si vous êtes sur `https://accounts.google.com`, Bitwarden remplira automatiquement le champ URL avec cette URL.*

6. - Le **bouton de gauche** permet de vérifier qu'il n'y ai pas eu de fuite de ce mot de passe. *Exemple : Facebook se fait pirater, les mots de passe sont dans la nature, Bitwarden permet de vérifier si ce mot de passe fait partie des données qui ont fuitées.*
	- Le bouton du milieu permet de voir votre mot de passe.
	- Le bouton de droite permet de générer ou de régénérer un mot de passe.
7. Ce bouton permet de générer un nom d'utilisateur ! Très utile, car une bonne pratique sur Internet est de ne pas utiliser les mêmes pseudos ! Ça permet de ne pas être identifié facilement.
8. N'oubliez pas de cliquer sur ce bouton ! C'est pour ***enregistrer*** !

## Installer l'application sur votre smartphone

Cherchez "**Bitwarden**" sur le Play Store pour Android ou sur l'AppStore pour IOS. Installez-le et connectez-vous.

L'application Bitwarden se verrouille automatiquement au bout de 15 minutes (vous pouvez le changer dans les paramètres, mais je vous conseille de le laisser par défaut).

Vous avez 4 onglets en bas de l'application. Cliquez sur ***Paramètres*** puis cliquez sur ***Services de remplissage automatique***, activez ***Services de remplissage automatique*** (ça vous enverra dans les paramètres de votre téléphone, et vous devrez manuellement accepter le **service de saisie automatique** pour Bitwarden) et ***Utilisez le remplissage automatique***.

Pour vous connecter plus facilement à l'application, je vous suggère d'activer "**Déverrouiller avec une empreinte digitale**" ou "**Déverrouiller avec un code PIN**" 

> Si vous choisissez le code pin, il vous affichera une fenêtre ou vous devez dire "oui" ou "non", cliquez ***"non"***, car si l'application est redemarrée, vous allez devoir remettre votre ***"mot de passe maître"***.


## Le générateur de mots de passe

Le générateur de mot de passe est très puissant et vous permet de générer des pseudos, des mots de passe et des phrases de passe. Je suis désolé pour l'image, c'est en anglais pour moi :

![Bitwarden Generateur](/bitwarden/bitwarden-generator.png)

1. Le **premier** bouton permet de copier le mot de passe, le **deuxième** permet d'en régénérer un nouveau.
2. Choisissez si vous voulez générer un mot de passe ou un nom d'utilisateur.
3. Choisissez si vous voulez générer un mot de passe ou une phrase de passe.
4. Options supplémentaires, je vous conseille de mettre le **nombre de mots à 6** pour la **phrase de passe**. Pour la séparation entre les mots, vous pouvez mettre ce que vous voulez (par défaut ça doit être un `-`, cliquez dessus et effacez-le si vous souhaitez mettre un espace comme moi), vous pouvez également mettre la première lettre de chaque mot en majuscule si vous le souhaitez.
5. C'est l'historique des mots de passe que vous avez générés, ils sont effacés à chaque fois que vous fermez votre navigateur web.

![Bitwarden Generateur password](/bitwarden/bitwarden-generator-password.png)

Dans le cas où vous avez choisi de générer un **mot de passe** au lieu d'une phrase de passe. Je vous conseille d'activer tous les boutons comme montré ci-dessus. Pour la longueur, choisissez une vingtaine de caractères, voire plus si vous le souhaitez.

## Les bonnes pratiques

1. Je vous conseille de ne jamais cliquer sur le bandeau qui s'affichera en haut de la page quand vous vous connecterez sur un site web que vous n'avez pas enregistré. Des erreurs sont parfois commises par Bitwarden !
Ajoutez manuellement vos identifiants à chaque fois, c'est beaucoup plus sûr !
2. Ne partagez ***sous aucun prétexte*** votre **`mot de passe maître`**.