---
title: "Les confusions face à la sécurité et la vie privée en ligne 🧐️"
date: 2023-05-06
---

Il faut premièrement ne pas confondre la vie privée et la sécurité.

La **vie privée** est le fait de garder certaines choses pour soi, ce ne sont pas forcément des secrets, ce sont juste les choses que vous ne souhaitez pas ou ne voyez pas l'intérêt de partager publiquement.

Tandis que la **sécurité** est l'action de protéger des actifs (des objets de valeur, des informations, des personnes, etc).

## #1 Tout est susceptible d'être piraté

Même si je vous propose des applications, des outils ou des smartphones de premier choix, cela ne veut pas dire qu'il est impossible que vous soyez piraté.

Il faut comprendre que la cybersécurité, c'est essentiellement une question de statistiques. En utilisant un [gestionnaire de mots de passe](/basiques/password-managers) tel que [Bitwarden](/fiches/biwarden) par exemple, vous réduisez drastiquement vos chances d'être piraté, contrairement aux bloc-notes physiques ou via une solution de bloc-notes en ligne (OneNote par exemple).

Cependant, cela ne signifie pas que Bitwarden est impossible à pirater. Il est tout à fait possible que cela arrive.
LastPass par exemple, un autre gestionnaire de mots de passe, s'est fait [piraté en août 2022](https://www.theverge.com/2023/2/28/23618353/lastpass-security-breach-disclosure-password-vault-encryption-update).

Les Google Pixel avaient une [faille vraiment effrayante](https://bugs.xdavidhu.me/google/2022/11/10/accidental-70k-google-pixel-lock-screen-bypass/) en 2022, car à la portée de tous, où vous aviez juste à insérer une carte SIM dont vous connaissiez le code PUK, erroner volontairement le code PIN de la carte SIM trois fois, taper le code PUK pour réinitialiser le code PIN (toujours de la carte SIM) et vous étiez dans le téléphone de votre victime (alors que vous êtes censé taper le code PIN du téléphone).

{{< youtube id="dSgSnYPgzT0">}}

## #2 L'effet de Halo

[L'effet de Halo](https://fr.wikipedia.org/wiki/Effet_de_halo) est un biais cognitif qui se manifeste lorsque l'on ressent un sentiment positif envers quelqu'un ou quelque chose influençant la perception que l'on a envers ses caractéristiques.

> **Exemple :** Si une personne est belle, on va tout de suite considérer qu'elle est intelligente et compétente alors qu'on ne l'a pas encore évalué sur ces points.

{{< youtube id="xJO5GstqTSY">}}

Cet effet s'applique également dans le monde de l'informatique.
Par exemple, si vous aimez utiliser un des produits que je propose sur mon site, ou que vous avez totalement confiance en la sécurité d'un de ces produits, vous allez penser que l'application est plus sécurisée que vous ne le croyez.

> **Exemple :** L’application [Signal](/fiches/signal) est une messagerie dite sécurisée, vos messages sont chiffrés de bout en bout et sont donc lisibles uniquement par le destinataire. Mais ce que vous ne devez pas oublier, c'est que Signal protège UNIQUEMENT le transport des messages, c'est à dire que si vous envoyez un message sensible à un de vos contacts et que ce contact souhaite le divulguer à tout le monde, ce n'est PAS le problème de Signal.

De même, si quelqu'un a accès à votre téléphone, il aura accès à tous vos messages sur Signal. Car Signal considère que vous devez sécuriser votre téléphone (ce qui est normal).

---

Il est important de ne pas extrapoler ce que vous voyez !

---

Il en va de même pour les marques (Google, Apple, etc...).
Vous aimez Apple pour sa simplicité ou son luxe, vous allez donc considérer qu'ils sont tout aussi excellents en cybersécurité ou pour la protection de votre vie privée. Si ils sont en effet très bons en termes de cybersécurité, certaines choses laissent encore à désirer en termes de vie privée...

## #3 Le principe de confiance

### VPN

Utiliser le moins de parties tiers possible est important pour votre vie privée et votre sécurité en ligne. L'exemple typique est le cas des VPNs : tout le monde vous vantent les bienfaits du VPN comme quoi votre FAI (Fournisseur d'Accès à Internet) ne pourra plus savoir ce que vous faites sur Internet ! Mais ce qu'ils ne disent pas, c'est que c'est maintenant votre fournisseur de VPN qui sait tout ce que vous faites en ligne !

Ce que vous avez fait ici s'appelle le déplacement de confiance (ou en anglais le "trust shifting"), vous avez déplacé la confiance que vous aviez en votre FAI vers votre fournisseur de VPN.

Quand je parle de confiance, je ne parle pas de confiance aveugle :

> "J'aime bien ce VPN, je lui fais confiance"

Je parle d'une confiance où l'on a lu les politiques de confidentialité, que l'on connaît qui gère l'organisation, que les fournisseurs sont transparents sur un ensemble de choses, etc...

Dans les deux cas, les deux types de fournisseurs ont accès à votre navigation web.

La confiance dans ce contexte n'est pas forcément positive, on doit juste faire confiance au moins d'entités possible.

La question se pose donc : "En qui avez-vous le plus confiance ?". Il faut donc regarder les lois françaises sur la protection des données, comment nos FAI gèrent-ils nos données contrairement à notre fournisseur de VPN, etc.

---

- [Les VPNs 🌍️ - SimplePrivacy](/basiques/vpn/)
- [Les VPNs et leur mésusage - Wonderfall](https://wonderfall.space/vpn-mesusage/)

---

### Antivirus

Sur Windows, vous avez un antivirus intégré nommé "Microsoft Defender", pourquoi faire confiance à un autre antivirus qui a son [lot de problèmes](https://wonderfall.space/windows-hardening/#microsoft-defender-antivirus) au lieu d'utiliser celui installé par défaut sur votre système. Microsoft Defender est le meilleur antivirus du marché, pour la simple et bonne raison qu'il est intégré à Windows, surtout qu'il fait bien plus qu'un antivirus. Pour rappel un antivirus n'est pas une solution de sécurité car il se base sur l'énumération du mal, qui est une méthode qui ne fonctionne pas dans le monde réel (le nôtre).

### Android et les Services Google Play

Je sais que c'est contre-intuitif, mais le fait d'acheter un Google Pixel permet de "gagner" en vie privée. Si les téléphones Android sont si terribles pour la vie privée des utilisateurs, c'est à cause de l'application "Services Google Play", elle est intégrée sur chaque système Android pour le grand public (Google Pixel, Samsung, OnePlus, Pocco, Xiaomi, Oppo, etc...). En utilisant un téléphone Samsung par exemple, vous faites confiance à Samsung et à Google en même temps (à cause des Services Google Play), alors qu'en utilisant un Google Pixel, vous ne ferez confiance qu'à Google.

Donc si vous souhaitez gagner en vie privée sans vous embêter, restez simple, prenez un Google Pixel, n'installez pas d'antivirus tiers et ne prenez pas de VPN.

> Je dis bien "pour faire simple", le mieux serait d'avoir un Google Pixel sous [GrapheneOS](https://grapheneos.org/), niveau vie privée, vous serez vraiment au top. Le VPN dépend énormément de vos besoins, mais les antivirus sont à proscrire.

## En savoir plus

### Evidence-based security et Antivirus

- 🇫🇷️ [Evidence-based Security - Wonderfall](https://wonderfall.space/evidence-based-security/)
- 🇬🇧️ [Knowledge Base - PrivSec](https://privsec.dev/posts/knowledge/)

### Les VPNs

- [Les VPNs 🌍️ - SimplePrivacy](/basiques/vpn/)
- [Les VPNs et leur mésusage - Wonderfall](https://wonderfall.space/vpn-mesusage/)

### Sécurité Android

- 🇫🇷️ [Le modèle de sécurité mobile - Wonderfall](https://wonderfall.space/modele-securite-mobile/)
- 🇬🇧️ [Features - GrapheneOS](https://grapheneos.org/features)
- 🇬🇧️ [Frequently Asked Questions - GrapheneOS](https://grapheneos.org/faq)
- 🇬🇧️ [The Android Platform Security Model](/assets/android-platform-security-model.pdf) ([Source originelle](https://dl.acm.org/doi/pdf/10.1145/344860))
- 🇬🇧️ [Android - Madaidan](https://madaidans-insecurities.github.io/android.html)
- 🇬🇧️ [Android Tips - PrivSec.dev](https://privsec.dev/posts/android/android-tips/) *(j'ai le même thème que son site web car c'est un thème publique et gratuit, ne soyez pas étonné)*
