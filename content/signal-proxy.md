---
title: "Serveur Proxy pour Signal"
date: 2022-09-24
---

## Proxy
[Signal est actuellement bloqué en Iran](https://signal.org/blog/run-a-proxy/), si vous souhaitez toujours utiliser Signal, je vous suggère d'utiliser Tor ou un VPN qui demande très peu d'informations vous concernant, comme [Mullvad](https://mullvad.net/en/).

Si dans votre pays, le réseau Tor, les VPN, et Signal sont bloqués, je vous conseille donc d'utiliser un proxy Signal.

J'héberge actuellement un proxy pour Signal. Pour éviter que les pays trouvent et bloquent mon proxy, je vous invite à m'envoyer un message privé sur [Element](https://matrix.to/#/@samsepi0l:arcticfoxes.net) ou via mon [adresse mail](mailto:contact@simpleprivacy.fr). Vous avez juste à demander pour mon proxy, je vous l'enverrai au plus vite (dans la journée) ou vous pouvez scannez le [QR code](https://twitter.com/SimplePrivacyFR/status/1573722737394302977) disponible sur mon [Twitter](https://twitter.com/SimplePrivacyFR/).
Vous avez ensuite juste à cliquer sur le lien depuis votre téléphone, cela ouvrira automatiquement Signal et vous demandera si vous souhaitez utiliser ce proxy. Après acceptation, vous serez connecté.

N'importe qui peut demander pour mon proxy, je vous suggère juste de ne le partager que par message privé. Cependant; ne le demandez uniquement que si Signal est bloqué dans votre pays, c'est inutile d'utiliser un proxy si Signal n'est pas bloqué.

D'autres serveurs proxy sont disponibles pour Signal sur Twitter en cherchant l'hashtag [#IRanASignalProxy](https://twitter.com/hashtag/IRanASignalProxy).

## Technologie

Pour ceux que ça intéressent, j'utilise l'[image docker](https://github.com/tommytran732/Signal-TLS-Proxy) de [Tommy qui a ajouté quelques améloriations de sécurité](https://privsec.dev/posts/proxies/update-your-signal-tls-proxy/).