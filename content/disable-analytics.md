---
title: Désactiver le tracking sur mon site
date: 2023-03-19
---

## Nota Bene
Tout d'abord, je tiens à vous rassurer que les données collectées sur ce site ne me permettent pas de vous identifier personnellement.
Vous pouvez voir les données collectées sur ce site [ici](https://plausible.simpleprivacy.fr/simpleprivacy.fr).

Si vous souhaitez tout de même refuser cette collecte, suivez ces instructions.

## Désactivation via Brave Shield

Sur le naviguateur Brave, accédez aux paramètres de Brave Shield [ici](chrome://settings/shields/filters) et copiez/collez ce [lien](https://plausible.simpleprivacy.fr/js/script.js) dans la zone de texte "**Créer des filtres personnalisés**" (1) puis enregistrez les modifications (2).

![Custom filter Brave shield](/disable-analytics/brave-filter.png)

Redémarrez Brave.

## Désactivation sur uBlock Origin

Sur les autres naviguateurs web, vous pouvez utiliser [uBlock Origin](https://ublockorigin.com).

Cliquez sur l'extension :

![click addon](/disable-analytics/click-addon.png)

Puis allez dans l'onglet "**Mes filtres**" puis dans la zone de texte, copiez/collez ce [lien](https://plausible.simpleprivacy.fr/js/script.js). 

![apply-filter](/disable-analytics/apply-filter.png)

Cliquez sur "Appliquer".

## Vérification

Pour vérifier que cela fonctionne, tapez la touche F12 de votre clavier, puis cliquez sur l'onglet "console", et **réactualisez** la page. Vous devriez voir une erreur comme quoi le lien https://plausible.simpleprivacy.fr/js/script.js n'a pas pu être chargé.
Si cette erreur est affiché, le script de Plausible n'enregistera rien de ce que vous faites.
Le tracking est donc désactivé.
