# Installer ou réinstaller le firmware

Cette documentation est valide pour les modèles suivants :
- Ironclad V3 (page produit : https://designedby.gg/product/ironclad-v3/)
- Berserker (page produit : https://designedby.gg/product/berserker/)
- Red Blade (page produit : https://designedby.gg/product/red-blade-01/)
- Dark Mage (page produit : https://designedby.gg/product/dark-mage-edition-qmk/)

## Comment identifier le firmware installé sur mon clavier ?

Attention : Ce paragraphe ne concerne pas le clavier Dark Mage, qui ne tourne que sur le firmware QMK.

Deux firmwares sont disponibles pour les claviers DbGG : le firmware d'origine dit "Evision", et QMK.

Plusieurs manipulations sont possibles pour identifier le firmware installé.

- Appuyez simultanément sur les touches Fn et Echap. Si le clavier s'éteint et ne réponds plus, QMK est installé (débranchez et rebranchez le clavier pour le rallumer).
- Débranchez et rebranchez le clavier. Si une animation en spirale de couleur blanche parcourt les touches, alors le firmware Evision est installé.
- Avec un navigatur web (hors Firefox), accédez au site https://usevia.app, et cliquez sur le bouton "Authorize device". Une popup doit s'ouvrir avec les périphériques pilotables par l'outil. Si votre clavier y est listé, QMK est installé. [[TODO screenshot VIA]]
- Si vous avez déjà installé le pilote du firmware d'origine Evision, il ne fonctionnera qu'avec celui ci. Si un message "Device not detected" y est affiché au lancement de l'application, QMK est le firmware installé. [[TODO screenshot driver]]

## Installer le firmware d'origine

Suivez la procédure indiquée sur la page suivante : TODO

## Installer le firmware QMK

Suivez la procédure indiquée sur la page suivante : [Installer QMK](https://github.com/Piefou/documentedbygg/blob/main/installer-firmware-qmk.md)
