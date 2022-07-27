---
title: "Les gestionnaires de mots de passe \U0001f511"
date: 2022-07-27
weight: 3
---

![Cadenas et clavier](/keys-and-keybinds.jpg)

Je préfère écrire la conclusion dès le début pour être sûr que ce soit clair pour tout le monde :

***Utilisez un gestionnaire de mots de passe, c'est la plus importante chose à faire sur toute votre vie numérique***

***Je vous conseille chaudement de lire [l'article de Wonderfall sur les mots de passe.](https://wonderfall.space/password/)***

*Je compte faire un tutoriel sur l'utilisation du gestionnaire de mots de passe **Bitwarden**, que je vous conseille fortement.
Ce sera un de mes prochains articles. Je rajouterai le lien vers ce guide en haut de cette page.*

## Les mots de passe

> Site web : Votre mot de passe ne comporte que des lettres !
> 
> Vous : Faut que je rajoute un caractère spécial en plus ???
>  
> Site web : Votre mot est passe est trop court !
> 
> Vous : Sérieusement ? Bon je vais rajouter ça

Cette situation a probablement déjà dû vous arriver, mais pourquoi ces sites web nous embêtent tant ? Et pourquoi je peux pas utiliser mon super mot de passe "monchat84" ?

Aujourd'hui, les mots de passe posent beaucoup de problèmes pour beaucoup de monde.
Un mot de passe permet de dire au service auquel vous vous connectez que vous êtes bien celui que vous prétendez être.

Cependant, trop de gens ont tendance à utiliser le même mot de passe sur tous leurs comptes, ou noter ça sur un post-it, ou pire encore, sur une application de prise de notes en ligne (tel que OneNote, Google Keep, un fichier Excel dans le Drive, etc.).

Le principe de mettre le même mot de passe partout est peut-être plus facile, mais si quelqu'un arrivait à vous pirater ou n'importe quel autre site auquel vous vous êtes connecté, vous perdez tous vos comptes !

Vous pouvez vérifier si vos identifiants ont été victime d'une fuite en allant sur [haveibeenpwned](https://haveibeenpwned.com/).

Juste pour que vous compreniez bien le problème d'utiliser le même mot de passe sur tous les comptes, je vais vous faire un exemple :

- Vous vous connectez avec le mot de passe `123456` sur Gmail.
- Puis avec le même mot de passe sur Netflix.
- Puis sur Linkedin.
- Puis... oooh, grosse faille sur Linkedin, vos mails et vos mots de passe sont dans la nature.

(Linkedin est un exemple fictif)

N'importe qui peut se connecter à n'importe lequel de vos comptes, puisque tout le monde a votre adresse mail et votre mot de passe.

Donc utilisez un mot de passe différent pour chaque site.

### Pourquoi un mot de passe doit comporter des majuscules et des caractères spéciaux ?

Tout simplement parce que cela augmente considérablement l'entropie du mot de passe. 

> Ah ! Toi aussi tu as vu Tenet ?

Pour expliquer simplement, l'entropie est la mesure du désordre.

En gros plus vous ajoutez des caractères spéciaux, des chiffres et des lettres, plus vous augmentez le désordre, donc par définition son entropie.

Il faut bien comprendre que ce n'est pas une personne qui va deviner un par un les mots de passe, mais des logiciels spécialisés pour ça. Il y a deux manières de cracker un mot de passe :

- L'attaque par **bruteforce**
- L'attaque par **dictionnaire**

Ces deux techniques peuvent être combinées.

Pour imager l'attaque par **bruteforce**, imaginez un cadenas à code à 4 chiffres. Le bruteforce est le fait de tester 0000, puis 0001, puis 0002 puis 0003 jusqu'à 9999, c'est long (pas pour un ordinateur évidemment), mais ça fonctionne.
Par exemple si votre mot de passe est `mot de passe`, le programme testera toutes les lettres, a puis b puis c jusqu'à z, puis continuera avec aa puis ab puis ac jusqu'à zz, etc. Notez bien que c'est un ordinateur qui fait ces calculs, le résultat sera donc très rapide. 

Pour imager l'attaque par **dictionnaire**, c'est comme le bruteforce, mais cette fois-ci avec des mots et non des carctères. Au lieu de faire caractère par caractère, le programme utilisera des mots couramment utilisé pour les mots de passe (des noms de famille, des métiers, des prénoms, des animaux, des lieux, etc.) tel que justement `mot de passe`. Le résultat sera instantané.

Voici un exemple de dictionnaire qu'on appelle aussi communément une **wordlist** :
[Wordlist française](https://raw.githubusercontent.com/scipag/password-list/main/countries/password-list-fr.txt).

Un programme utilisera ce fichier comme base, puis on y ajoutera certains paramètres à ce programme comme :

- les a peuvent être des @ ou des 4
- les E peuvent être des 3
- les o peuvent être des 0 (zéro)

> Donc oui, `m0t de p@sse` ne vous aidera pas non plus.

Il est important de noter que même si votre mot de passe ressemble à ça :

> t4@#L"5A

Il peut être deviné (par un ordinateur) en quelques minutes seulement, alors que pourtant, le mot de passe contient tout ce que les sites web demandent :

- [x] 8 caractères
- [x] Chiffres
- [x] Majuscules
- [x] Minuscules
- [x] Caractères spéciaux

Le problème que beaucoup de gens et de sites web oublient, c'est que l'entropie du mot de passe ne se joue pas uniquement sur sa complexité, mais également et **surtout** sur sa longueur.

> Au passage si votre mot de passe fait moins de 8 caractères, c'est cracké en quelques secondes, voir moins d'une seconde.

 Un bon mot de passe est un mot de passe qui est complexe et qui long. Si votre mot de passe ressemble à ça :

> aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa

C'est super long, mais c'est devinable en moins d'une seconde pour un ordinateur. D'où l'importance de la complexité du mot de passe.

Un bon mot de passe serait quelque chose comme ça :

> @UpXg$atJqQue@x43C8B&matxz4Ed&!C

Mais t'es malade, comment crois-tu que je vais retenir ça ???

En effet, c'est compliqué à retenir. On peut cependant changer ça très simplement en écrivant des phrases et non des mots de passe. Voire mieux, utilisez un gestionnaire de mots de passe.

## Les phrases de passe

![xkcd entropie](/xkcd-entropie.png)
*L'image vient de [xkcd](https://xkcd.lapin.org/index.php?number=936#strips)*

*Je vous recommande encore une fois [l'article de Wonderfall](https://wonderfall.space/password/) qui explique très bien cette image*

Les phrases de passe sont une excellente manière (pour un humain) de retenir ses mots de passe simplement tout en ayant une entropie élévée.

On a la chance d'être français, car nous possédons beaucoup de caractères spéciaux dans notre langue, tel que justement :

- le ç
- l'apostrophe
- les lettres avec accent (é, è, à, etc.).

Notez aussi que l'espace est un caractère spécial exactement comme le `#` ou le `!`. Écrivez ces phrases dans le champ de mot de passe comme si vous écriviez la phrase en vrai (la majuscule au début, les espaces, le point à la fin et les apostrophes).

Donc une phrase de passe comme :

> J'ai mangé une côte de boeuf à 15 €.

est parfaitement viable. (N'oubliez quand même pas de rajouter des chiffres). C'est viable, car le mot de passe respecte les conditions :

- [x] 36 caractères
- [x] 2 chiffres (`15`)
- [x] La majuscule (`J`)
- [x] Les minuscules
- [x] Les caractères spéciaux ( l'apostrophe `'`, les espaces ` `, le `é`, le `ô`, le symbole `€` et le point final `.`)

On voit tout de suite que c'est plus facile à retenir qu'un mot de passe de 35 caractères.

![Dés](/dices.jpg)

Cependant, la phrase reste prévisible, et une bonne phrase de passe ressemblerait plutôt à ça (aussi appelé diceware) :

> timing paving hertz bacterium pliable angelfish

Qui est également le titre de [l'article de Wonderfall](https://wonderfall.space/password/) que je vous recommande vivement.

Tous ces mots sont générés aléatoirement (par un ordinateur, et non par un humain). Il n'y a pas de majuscules ou de chiffres, mais il possède 6 mots générés **complètement aléatoirement**.

Vous pouvez générer des phrases de passe avec [ce site](https://www.rempe.us/diceware/#french) afin de tester un peu. Cependant, c'est mieux de générer votre phrase de passe avec votre gestionnaire de mots de passe. Bitwarden est capable de générer une liste de mots par exemple.

Pour vous donner une idée, un ordinateur personnel est capable de tester quelques millions de mots de passe par seconde.
Vous devez supposer qu'une personne mal intentionné peut aller jusqu'à tester un billion de mots de passe par seconde (soit mille milliards) si il en a les moyens. 

La phrase de passe comme plus haut, contient 6 mots, et prendrait environ 3500 ans à cracker en testant un billion de mots de passe par seconde. Rajouter un autre mot comme ceci (pour arriver à 7) : 

> timing paving hertz bacterium pliable angelfish massue

Et vous passez à 27 millions d'années de calculs. Cependant, si vous passez de 6 à 5 mots :

> timing paving hertz bacterium pliable

On passe de 3500 ans (pour 6 mots) à 5 mois en testant un billion de mots de passe par seconde.

*Ces infos proviennent directement du site [diceware](https://www.rempe.us/diceware/#french)*

La meilleure solution serait la phrase de passe, couplé avec un gestionnaire de mots de passe.

> Bitwarden propose la génération d'une phrase de passe composé de 3 mots par défaut séparé par un `-`, je vous conseille de le paramétrer à 6 mots. Vous pouvez aussi, si vous le souhaitez, activer les majuscules au début de chaque mot et ajouter un chiffre.

Un humain pourra d'ailleurs plus facilement retenir une liste de mots qu'une suite de caractères incompréhensibles.

Le minimum requis serait [6 mots](https://wonderfall.space/password/#calculs-dentropie) à mon opinion. **Avec un espace ou n'importe quel autre caractère spécial entre les mots**

*Si un site web n'accepte pas plus de 20 caractères, vous serez incapable de faire plus de 3 mots. Je vous conseille de générer un mot de passe aléatoire.*

## Les gestionnaires de mots de passe

Même en utilisant des phrases de passe, il vous reste un problème majeur : il faut avoir un mot de passe différent par site web.
Et c'est compliqué, voire impossible de tous les retenir.

Plusieurs solutions s'offrent à vous :

1. La solution papier : écrire sur un post-it ou un sur carnet.
2. L'écrire dans une application de prise de notes de type OneNote, Google Keep, ou dans un fichier Excel.
3. Utiliser un gestionnaire de mots de passe.


### La solution papier

Le problème d'écrire sur un post-it ou carnet est que n'importe qui peut juste l'ouvrir et lire vos mots de passe et mail. Vous allez vous dire que vous avez juste à écrire votre mail de cette façon :

> sam-----@--.com

Mais ça ne vous aidera pas plus, beaucoup de gens utilisent le même mail pour tous leurs comptes également, donc cacher son mail n'est pas très utile. Surtout que c'est une info qui peut être retrouvée facilement sur Internet.
Si vous commencez à vous dire que vous pouvez toujours décaler les caractères de vos mots de passe (par exemple `a` devient `b` ou `1` devient `2`), ou que vous omettez un caractère que vous ajoutez manuellement pendant la connexion du site, laissez-vous dire que vous vous prenez la tête pour très peu de sécurité et de commodité.

### Les applications de prise de notes

Mettre votre mot de passe sur une application comme Google Keep est une aberration pour plusieurs choses.

La première est que ces applications ne sont pas faites pour enregistrer des identifiants. Vos données sont dans le cloud et votre fournisseur **voit** ces données en clair (Google, ou Microsoft (OneDrive), etc.). Comme ce n'est pas chiffré, si un hacker compromet un des serveurs, il aura accès à tous vos mots de passe.

La deuxième, c'est que vous avez rarement un mot de passe à entrer pour accéder à votre application, si vous utilisez OneNote sur le téléphone par exemple, une fois connecté, vous restez connecté. Donc si vous laissez votre smartphone à quelqu'un ou ouvert sur une table en soirée, une personne peut juste aller sur votre téléphone et voler vos mots de passe. Ne minimisez pas le fait qu'il y ai peu de chances que ça arrive, c'est une menace réelle.

### Les gestionnaires de mots de passe

Les gestionnaires de mots de passe sont souvent sous forme d'extension sur votre navigateur (Firefox, Google Chrome, Brave, Safari) vous cliquer sur l'extension puis cliquez sur l'identifiant et ça remplit automatiquement les champs de texte !

Si vous ne faites pas confiance aux gestionnaires de mots de passe parce que ça revient à dire que vous mettez tous vos oeufs dans le même panier. Le problème est exactement le même en utilisant une application de prise de notes ou en utilisant le même mot de passe partout. Et puis pourquoi faire confiance à OneNote ou Google Keep si vous ne faites pas confiance au gestionnaire de mots de passe ? 

La différence est qu'un gestionnaire de mots de passe est fait pour ça, il implémente du chiffrement de bout en bout, et **vous seul** uniquement, avez accès à vos identifiants. Ni le gestionnaire de mots de passe ni un hacker pourrait voir vos identifiants, car tout est chiffré et vous seul avez la clé.

Et puis les gestionnaires de mots de passe sont fait pour être simple, vous cliquez sur un bouton, et ça vous remplis automatiquement la page. Vous pouvez générer des mots de passe complexes, rajoutez des notes à vos identifiants, ajoutez vos carte bancaires, etc. Vous pouvez également installer Bitwarden sur votre PC (ou MacBook), sur votre smartphone (ou iPhone), et si vous êtes en sortie, que vous n'avez ni votre PC et ni votre smartphone vous pouvez directement accéder sur un navigateur !
Je sais que Bitwarden le fait, vous pouvez y accéder en allant sur [vault.bitwarden.com](https://vault.bitwarden.com).

Les gestionnaires de mots de passe sont sécurisés, et super pratiques ! Donc utilisez-les !

### Quel gestionnaire utiliser ?

**[Bitwarden](https://bitwarden.com/)** : c'est gratuit, c'est open source, c'est simple.

Pour ceux qui voudraient un gestionnaire de mots de passe uniquement en local, je vous conseille [Keepass](https://keepass.info/).

Mais vous devriez quand même utiliser les solutions cloud comme Bitwarden. Puisque si vous voulez utiliser un gestionnaire de mots de passe, vous devez faire attention à ce que votre réseau à la maison soit suffisamment protégé, votre appareil aussi, etc.

> *Je rappelle qu'aucun produit n'est affilié, je choisis les solutions selon leurs mérites. J'utilise Bitwarden tous les jours, car à ma connaissance, c'est le seul gestionnaire de mots de passe open source qui propose autant de simplicité et de fonctionnalités.*

### Comment ça fonctionne

Vous vous créez un compte sur **Bitwarden** par exemple.
Vous créez une phrase de passe (également appelé *master password*) pour être capable de le retenir (vous pouvez ajouter un caractère spécial en plein milieu d'un des mots comme `J'ai mangé` devient `J'ai man?gé` juste pour bien embêter le monde) et vous ajoutez vos identifiants de vos comptes.

Un gestionnaire de mots de passe est basiquement une liste de vos mots de passe, chiffrés, que vous seul avez accès.

Je vais redire ce que j'ai dit dans mon [article](/basics/threat-model/#prot%C3%A9ger-votre-vie-priv%C3%A9e-des-fournisseurs-de-services) sur la [modélisation des menaces](/basics/threat-model).

*Je vais simplifier énormément les faits évidemment, mais ça permettra que tout le monde comprennent de quoi je parle.*

![Image explicative](/bank-example.png)

Vous avez un coffre à la banque, ce coffre est le numéro 1, les autres coffres sont à d'autres clients de la banque.

Le problème étant que si c'est la banque qui gère votre clé, elle peut ouvrir votre coffre à n'importe quel moment, de plus si des braqueurs arrivent dans la banque, ils n'ont qu'à voler les clés, et ouvrir les coffres de tout le monde !

Pour ce faire, la banque va vous donner une clé, vous serez le seul à avoir cette clé et personne d'autre. Quand vous voudrez aller à la banque pour ouvrir votre coffre, vous pourrez l'ouvrir grâce à l'unique clé que vous détenez.

C'est exactement le même principe avec les gestionnaires de mot de passe.

Votre banque est le gestionnaire de mots de passe, et les coffres sont les bases de données chiffrées des personnes.

> Une base de données est une liste d'informations, ici, ce sont des identifiants de connexion. Mais vous pouvez imaginer ça comme une feuille Excel par exemple.

Quand vous vous connectez à **Bitwarden** par exemple, vous donnez votre mail et votre `master password` et ça va permettre d'identifier à qui appartient telle base de données.

Bitwarden vous enverra votre base de données sur votre navigateur (toujours en chiffré) et tout sera déchiffré localement au niveau de votre navigateur.

Si vous souhaitez en savoir plus je vous conseille d'aller voir ces liens, tous en anglais :

- [How password managers work - Computerphile](https://www.youtube-nocookie.com/embed/w68BBPDAWr8) (Vidéo YouTube)
- [How to choose a password - Computerphile](https://www.youtube-nocookie.com/embed/3NjQ9b3pgIg) (Vidéo YouTube)
- [Bitwarden Docs - Vault Data](https://bitwarden.com/help/vault-data/)
- [Bitwarden Docs - What encryption is used](https://bitwarden.com/help/what-encryption-is-used/)
- [Page Cryptographique Interactive par Bitwarden](https://bitwarden.com/crypto.html)

## Les bonnes pratiques

Une fois que vous avez un gestionnaire de mots de passe tel que Bitwarden. Certaines bonnes pratiques sont quand même à prendre en compte.

1. Si vous vous connectez sur [vault.bitwarden.com](https://vault.bitwarden.com) ou n'importe quel autre gestionnaire de mots de passe accessible en ligne. Pensez à ouvrir un nouvel onglet privé, car une fois que vous fermerez cette fenêtre, vous serez déconnecté de l'appareil. Au pire des cas, la version web de Bitwarden vous déconnecte automatiquement au bout de 15 minutes, vous pouvez raccourcir ce temps dans les paramètres de votre compte.
2. Pensez à créer un mot de passe unique (une vingtaine de caractères aléatoires est déjà pas mal) sur chaque site web que vous visitez.
3. Ne donnez sous aucun prétexte votre `master password` à qui que ce soit !

## Credits

- [How password managers work - Computerphile](https://www.youtube-nocookie.com/embed/w68BBPDAWr8) (Vidéo YouTube)
- [How to choose a password - Computerphile](https://www.youtube-nocookie.com/embed/3NjQ9b3pgIg) (Vidéo YouTube)
- [timing paving hertz bacterium pliable angelfish - Wonderfall](https://wonderfall.space/password/)
