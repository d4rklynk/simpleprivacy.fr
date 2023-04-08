---
title: Politique de confidentialité
date: 2022-07-25
---

## Version simple :

Rien n'est collecté.

## Version longue :

Je me fiche de qui vous êtes, ou de ce que vous faites sur mon site web.
Je suis là pour partager mes connaissances, et non vos données.

## Version plus longue :

### Hébergeur web
J'utilise Google Domains pour le nom de domaine et les serveurs DNS. J'utilise Netlify pour héberger le site web.

Netlify garde votre adresse IP dans leurs logs pendant un maximum de 30 jours, vous pouvez en savoir plus en visitant ce [lien](https://www.netlify.com/gdpr-ccpa/). Leur politique de vie privée peut se trouver [ici](https://www.netlify.com/gdpr-ccpa/).

### Locigiels
J'utilise [hugo](https://gohugo.io/) pour la génération du site. Hugo possède quelques [paramètres concernant la vie privée](https://gohugo.io/about/hugo-and-gdpr/) pour être en règle avec la [RGPD](https://www.cnil.fr/fr/comprendre-le-rgpd), j'ai [configuré ces paramètres](https://github.com/d4rklynk/simpleprivacy.fr/blob/main/config.yml#L159) afin qu'il y est le moins d'impact possible sur votre vie privée.

Les services tels que Disqus (intégration de commentaires), Instagram et Google Analytics sont désactivés. Certains liens vous redirigeront vers Twitter et Youtube à travers le site, les options "[enableDNT](https://github.com/d4rklynk/simpleprivacy.fr/blob/main/config.yml#L172)" et "[privacyEnhanced](https://github.com/d4rklynk/simpleprivacy.fr/blob/main/config.yml#L180)" sont par conséquent activés pour ces services.

### Dépot Git
J'utilise GitHub afin d'héberger [mon dépot](https://github.com/d4rklynk/simpleprivacy.fr). Si vous souhaitez contribuer à mon site web, vous devrez créer un compte GitHub.
Vous pouvez lire leur politique de vie privée [ici](https://docs.github.com/fr/site-policy/privacy-policies/github-privacy-statement).
