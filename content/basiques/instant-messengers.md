---
title: "Les messageries instantanées et le chiffrement de bout en bout \U0001f910"
date: 2022-08-08
---

![Messageries instantanées](/instant-messengers/instant-messengers.jpg)

Les messageries instantanées sont des solutions de communication incontournables au 21ème siècle.

Je vais vous expliquer le fonctionnement de ces messageries. Mais d'abord vous devez comprendre ce qu'est le chiffrement de bout en bout.

## Le chiffrement de bout en bout

Le chiffrement de bout en bout consiste à chiffrer les messages à partir des appareils des utilisateurs, c'est à dire que si vous utilisez votre application sur votre téléphone, le message sera chiffré à partir de votre application de votre téléphone, et sera déchiffré uniquement sur l'application du destinataire, aucun tiers pendant le transit du message n'est capable de savoir le contenu du message.

Pour comprendre, je vais vous expliquer avec un exemple de la poste.

![Image exemple poste](/instant-messengers/mail-exemple.png#center)

Alice envoie une carte postale à Bob, le service de la poste s'occupera du transfert de cette carte postale.
Le problème dans ce cas, c'est que la carte postale n'est pas dans une enveloppe, elle n'est pas scellée, n'importe qui peut lire ou modifier la carte avant que Bob la réceptionne.

Trois problèmes majeurs se posent :

- **Confidentialité**
- **Intégrité**
- **Authenticité**

Tout le monde peut lire le message, Alice, Bob, et toute autre personne a accès à cette carte postale. La ***confidentialité*** n'est pas assurée car seuls Alice et Bob devraient avoir connaissance du message.

Bob ne peut pas vérifier que le message de la carte postale est ***intègre***. C'est à dire qu'on ne peut pas garantir que le message n'a pas été modifié par une tierce personne pendant le transit de la carte.

Bob ne peut pas vérifier l'***authenticité*** de la carte car on ne peut pas être certain que c'est bien Alice qui a envoyé le message, et non une tierce personne.

---

Ces trois problèmes peuvent cependant être réglés facilement.

---

- Pour la **confidentialité** du message, Alice peut chiffrer son message grâce à un code secret déjà établi entre Alice et Bob. Si une tierce personnne lisait la carte postale d'Alice, cette personne ne comprendrait rien ! Seuls Alice et Bob se comprendraient !
- Pour l'**intégrité** de la carte, Alice peut tracer deux petits traits à l'arrière de l'enveloppe. Quand Bob recevra l'enveloppe, si les traits sont bien alignés, c'est que l'enveloppe n'a pas été ouverte et donc que le message est intègre.
- Pour l'**authenticité**, Alice peut signer sa carte postale, ou au dos de l'enveloppe pour prouver que c'est bien elle qui a écrit le message.

### Fonctionnement du chiffrement

Le principe du chiffrement de bout en bout repose sur le chiffrement dit **asymétrique**.

![Génération des clés](/instant-messengers/keygen.png#center)

Le principe repose sur la génération d'une **paire de clés**, une clé **publique** et une clé **privée**. Alice va générer sa paire de clé, donc une clé publique (en vert) et une clé privée (en rouge). Bob fera de même en générant sa clé publique (en vert) et sa clé privée (en bleu). Dites-vous que ces deux clés (publique et privée) sont comme des faux jumeaux, elles sont intimement liées, mais ne se ressemblent pas.

La clé **publique** est, comme son nom l'indique, publique. Vous pouvez la donner à vos amis, à votre famille, sur Internet, sur les réseaux sociaux, etc. C'est la clé qui permettra aux autres de ***chiffrer*** les messages qui vous sont destinés (puisque la clé publique est reliée à votre clé privée, donc vous).

La clé **privée** est, comme son nom l'indique, privée. Vous devez ***absolument*** garder cette clé pour vous, vous ne devez pas la partager ! C'est la clé qui permettra de ***déchiffrer*** les messages qui vous sont destinés (puisque les gens auront chiffré leur message avec votre clé publique).

![Bob à Alice](/instant-messengers/encryption-message.png#center)

Si **Bob** veut envoyer un message à Alice, Bob doit avoir la clé publique **d'Alice** (`Alice PUB` dans l'image) pour pouvoir communiquer avec elle. Bob va donc **chiffrer** son message avec la **clé publique d'Alice**, puis une fois envoyé, Alice **déchiffrera** le message avec sa **clé privée à elle** (`Alice PRIV` dans l'image).

Si Alice envoyait un message à Bob, Alice devrait se procurer la **clé publique de Bob** pour pouvoir chiffrer son message, puis Bob déchiffrerait le message avec sa **clé privée à lui**.

Une conversation normale ressemblerait donc à ça :

![Conversation chiffrée](/instant-messengers/encrypted-conversation.png#center)

Les messageries instantanées (certaines) implémentent donc le chiffrement de bout en bout pour assurer la **confidentialité** des messages. Mais les clés privées permettent également de garantir l'[authenticité](#la-signature-digitale) des messages !

---

Le **chiffrement** garantit la **confidentialité**.

---

Je vous envoie sur les sites de la [CNIL](https://www.cnil.fr/fr/) pour en savoir plus, deux articles sont disponibles :

- [Sécurité : Chiffrer, garantir l’intégrité ou signer - CNIL](https://www.cnil.fr/fr/securite-chiffrer-garantir-lintegrite-ou-signer)
- [Comprendre les grands principes de la cryptologie et du chiffrement- CNIL](https://www.cnil.fr/fr/comprendre-les-grands-principes-de-la-cryptologie-et-du-chiffrement) (je vous conseille fortement de lire cet article, il est complet et facile à comprendre)

### Le hachage

Le **hachage** est un procédé informatique par lequel on hache une donnée (un fichier, message, etc), de la même manière qu'un steak haché par exemple. On a donc ensuite le **fichier d'origine** et le **fichier haché**, qui est l'empreinte digitale numérique du fichier d'origine. Plusieurs algorithmes de hachage existent, voici le hash du mot `France` avec plusieurs algorithmes de hachage différents :

- **MD5 :** `0309a6c666a7a803fdb9db95de71cf01`
- **SHA1 :** `e3772ac4b4db87b4a8dbfa59ef43cd1a8ad29515`
- **SHA256 :** `7a1ca4ef7515f7276bae7230545829c27810c9d9e98ab2c06066bee6270d5153`

Si vous changez `France` en `france`, vous obtenez des résultats complétement différents :

- **MD5 :** `e165d4f2174b66a7d1a95cb204d296eb`
- **SHA1 :** `23e591e8c36dda987970603ad0fdd031b7dff9f9`
- **SHA256 :** `2c598436e5575a5769b69986014588d52c2698414b623e81b2e776766c30eaba`

Même si quelque chose de minime est changé, le hash (le résultat du hachage) sera complètement différent. Donc si Alice chiffre son message puis le hache, elle enverra son message et le hash à Bob, et Bob n'aura plus qu'à lui aussi hacher le message et vérifier que c'est le même résultat que le hash envoyé par Alice. Si c'est le cas, le message n'as pas été modifié, sinon, Alice doit renvoyer son message (avec le hash).

---

Le **hachage** garantit l'**intégrité**.

---

### La signature digitale

La **signature** est générée grâce à une clé privée, et peut être vérifiée avec une clé publique (de celui qui l'a signé).

Quand Alice souhaite générer une signature, elle va **chiffrer** la donnée (document, mails, message, ...) avec **sa clé privée à elle** (et non avec la clé publique de quelqu'un d'autre).

Si Alice souhaite envoyer un message à Bob, elle utilisera **la clé publique de Bob** pour **chiffrer** son message et **sa clé privée à elle** pour **signer** ce message, quand Bob recevra le message chiffré d'Alice, il **déchiffrera** le message avec sa **clé privée à lui** et vérifiera la **signature** du message grâce à la **clé publique d'Alice**.

---

La **signature digitale** garantit l'**authenticité**.

---

Une vidéo en anglais est disponible sur YouTube pour comprendre la signature digitale :

- [What are Digital Signatures? - Computerphile](https://www.youtube.com/watch?v=s22eJ1eVLTU)

## On dit chiffrer, et pas crypter

Tant qu'on y est, "crypter" n'est pas français.

- **Chiffrement** : chiffrer un message **grâce** à une clé.
- **Déchiffrer** : déchiffrer un message **grâce** à une clé.
- **Décrypter** : déchiffrer un message **sans** la clé (un hacker qui essayerait de découvrir le contenu du message par exemple).
- **Crypter** : chiffrer un message **sans** la clé (???).

Je vous envoie sur ce site très bien fait qui explique les différences entre les termes :

- [On dit chiffrer, et pas crypter - Max](https://chiffrer.info/)

---

Maintenant que vous avez compris ces notions, je vais vous présenter différentes messageries instantanées.

---

## Facebook Messenger

[Facebook Messenger](https://www.messenger.com/?locale=fr_FR) fonctionne de cette manière :

![Facebook Messenger exemple](/instant-messengers/facebook-messenger.png#center)

Quand Alice envoie un message à Bob, l'application Messenger envoie le message aux serveurs de Facebook. Ce message reste stocké sur ce serveur. L'application Messenger de Bob va demander au serveur de voir le message, le serveur lui envoie une copie de ce message, et Bob sera en mesure de lire le message d'Alice.
Le message d'Alice est toujours sur le serveur.

Le problème est que sur Facebook Messenger, les messages ne sont pas chiffrés de bout en bout, et sont donc visibles par Facebook puisque les messages restent stockés sur leurs serveurs. C'est une gigantesque intrusion à votre vie privée, et cela revient à la même chose que si vouz étiez à la terrasse d'un café avec l'une de vos amies, et qu'au lieu de parler tranquillement, vous discutiez en hurlant.

Une fonctionnalité appelée "conversation secrète" est disponible sur Facebook, mais est à mon sens inutile puisque Facebook collecte massivement vos métadonnées de cette "conversation secrète". Je vous conseille d'abandonner Facebook Messenger et d'utiliser [Signal](#signal).

## WhatsApp

[WhatsApp](https://www.whatsapp.com/?lang=fr) fonctionne autrement :

![WhatsApp exemple](/instant-messengers/whatsapp.png#center)

Quand Alice souhaite envoyer un message à Bob, le message sera **chiffré** puis envoyé aux serveurs de WhatsApp. Les serveurs ne servent qu'à délivrer le message. Les messages restent stockés sur les serveurs uniquement le temps de la livraison du message. Une fois que Bob à reçu le message, il est supprimé du serveur et les messages restent stockés sur les appareils d'Alice et Bob.

Une [surface d'attaque](https://fr.wikipedia.org/wiki/Surface_d%27attaque) présente sur WhatsApp est le fait que les images et les vidéos sont automatiquement enregistrées sur l'appareil. Jeff Bezos (le PDG d'Amazon) [s'est fait piraté](https://www.theguardian.com/technology/2020/jan/21/amazon-boss-jeff-bezoss-phone-hacked-by-saudi-crown-prince) de cette manière. Je vous conseille de **désactiver** cette fonctionnalité.

> WhatsApp utilise le "[Signal Protocol](https://www.whatsapp.com/security/WhatsApp-Security-Whitepaper.pdf)". Cependant, le "Signal Protocol" ne garantit pas que les **métadonnées** soit chiffrées.

Sur WhatsApp, les métadonnées ne sont pas chiffrées, et donc visibles par WhatsApp (et donc Facebook), telles que l'heure exacte de l'envoi de vos messages, à qui, combien de fois, pendant combien de temps, etc.
Les métadonnées sont [aussi importantes que les données](https://ssd.eff.org/fr/module/voici-pourquoi-les-m%C3%A9tadonn%C3%A9es-sont-importantes). Si vous êtes une femme et que vous parlez à un homme depuis quelques mois, et ce, tous les jours, on se doute que vous êtes en couple depuis peu. Si ensuite vous allez voir sur Facebook la page d'un restaurant, puis vous envoyez un message à vos parents, on suppose que vous allez présenter votre nouveau partenaire à vos parents. Dans les faits, c'est probablement encore plus simple, car on sous-estime énormément ce que sont les métadonnées.

Même si vos messages sur WhatsApp sont chiffrés, on n'a pas besoin de connaître le contenu des messages pour connaître votre vie.

En archéologie par exemple, on peut deviner l'utilité d'un objet grâce aux métadonnées : la composition de l'objet, à quelle date tel métal était utilisé, le type d'objet, etc. Donc oui les métadonnées ne sont pas anodines.

## Telegram

[Telegram](https://telegram.org/?setln=fr) ne propose pas de chiffrement de bout en bout par défaut (comme Facebook Messenger). Les messages restent sur les serveurs et sont donc visibles par Telegram.

De plus, Telegram utilise son propre protocole qui n'a pas été audité. Telegram est le seul à l'utiliser, ce protocole est propriétaire, on n'a donc aucune idée ce qu'il fait.

Des experts en sécurité ont trouvé [plusieurs failles](https://portswigger.net/daily-swig/multiple-encryption-flaws-uncovered-in-telegram-messaging-protocol) au protocole de Telegram.
Un [chapitre en anglais](https://madaidans-insecurities.github.io/messengers.html#telegram) a déjà été écris concernant les problèmes de Telegram.

## Wire

[Wire](https://wire.com/en/) est [open source](https://github.com/wireapp) et a été [audité](https://wire.com/en/blog/application-level-security-audits/). Cependant toutes les métadonnées restent en clair sur leurs serveurs. Ce qui est encore un problème majeur.

## Signal

[Signal](https://www.signal.org/fr/#signal) est l'application par excellence, elle est utilisée par [Edward Snowden](https://mobile.twitter.com/Snowden/status/661313394906161152), les [métadonnées sont protégées](https://signal.org/blog/sealed-sender/). Les [seules métadonnées](https://signal.org/bigbrother/eastern-virginia-grand-jury/) que Signal possède d'un utilisateur sont la date et l'heure de création du compte et la dernière fois qu'il s'est connecté sur leurs services. Oui, c'est rien. Et leur [protocole](https://www.signal.org/docs/) ("**The Signal Protocol**") est un standard de nos jours (la preuve est que [WhatsApp l'utilise](https://www.whatsapp.com/security/WhatsApp-Security-Whitepaper.pdf) depuis des années).

Beaucoup d'experts en sécurité ont toujours recommandé Signal.

Je ne suis pas un expert, mais je vous recommande Signal également, en plus c'est super simple à utiliser, vous avez autant de fonctionnalités que WhatsApp, voire plus.

## Conlusion

Utilisez [Signal](https://www.signal.org/fr/#signal). Le "[Signal Protocol](https://www.signal.org/docs/)" garantit **authenticité**, **intégrité** et **confidentialité**.

---

## En savoir plus & crédits

### Sur la cryptographie (authenticité, intégrité, confidentialité)

- [Sécurité : Chiffrer, garantir l’intégrité ou signer - CNIL](https://www.cnil.fr/fr/securite-chiffrer-garantir-lintegrite-ou-signer)
- [Comprendre les grands principes de la cryptologie et du chiffrement- CNIL](https://www.cnil.fr/fr/comprendre-les-grands-principes-de-la-cryptologie-et-du-chiffrement)
- [On dit chiffrer, et pas crypter - Max](https://chiffrer.info/)
- [End to End Encryption (E2EE) - Computerphile](https://www.youtube.com/watch?v=jkV1KEJGKRA)
- [Secret Key Exchange (Diffie-Hellman) - Computerphile](https://www.youtube.com/watch?v=NmM9HA2MQGI)
- [Double Ratchet Messaging Encryption - Computerphile](https://www.youtube.com/watch?v=9sO2qdTci-s)
- [What are Digital Signatures? - Computerphile](https://www.youtube.com/watch?v=s22eJ1eVLTU)

### Sur les messageries instantanées

- [How Signal Instant Messaging Protocol Works (& WhatsApp etc) - Computerphile](https://www.youtube.com/watch?v=DXv1boalsDI)

- [What's Up With Group Messaging? - Computerphile](https://www.youtube.com/watch?v=Q0_lcKrUdWg)

- [Messengers - Madaidan](https://madaidans-insecurities.github.io/messengers.html)

### Sur les métadonnées

- [Voici pourquoi les données sont importantes - EFF](https://ssd.eff.org/fr/module/voici-pourquoi-les-m%C3%A9tadonn%C3%A9es-sont-importantes)