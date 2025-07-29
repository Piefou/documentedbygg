# Installer le firmware QMK

Cette documentation est valide pour les modèles suivants :

- Ironclad V3 (page produit : https://designedby.gg/product/ironclad-v3/)
- Berserker (page produit : https://designedby.gg/product/berserker/)
- Red Blade (page produit : https://designedby.gg/product/red-blade-01/)
- Dark Mage (page produit : https://designedby.gg/product/dark-mage-edition-qmk/)

## Préparer les fichiers nécessaires

Pour installer le firmware QMK, vous aurez besoin de plusieurs fichiers :
- L'outil de flash qui va appliquer le nouveau firmware
- Le fichier binaire du firmware à installer
- Le fichier JSON à charger dans VIA

L'outil de flash est disponible sur la page Github suivante : https://github.com/SonixQMK/sonix-flasher/releases
Pour la dernière release, récupérez l'archive correspondant à votre OS :
- flasher-win.zip pour Windows
- flasher-mac.dmg pour MacOS
- flasher-linux.tar.xz pour une distribution Linux

Vous y trouverez l'outil de flash sous la forme d'un exécutable dans le dossier "Sonix Keyboard Flasher" de l'archive.

Les fichiers supplémentaires dépendent de votre clavier, et sont rassemblés dans les archives suivantes :
- Dark Mage : [Lien](downloads/darkmage-qmk-20250729-caps-lock.zip)

Décompressez également cette archive, qui contient un fichier BIN et un fichier JSON.

Débranchez tout autre clavier "custom" de votre ordinateur.

## Procédure d'installation

Attention !
Une mauvaise exécution de la procédure peut rendre inopérant votre clavier. Lisez bien une première fois l'intégralité des manipulations avant de vous lancer, et ne deviez pas des instructions. Si vous avez un doute, n'hésitez pas à demander sur le Discord.

Le début de la procédure dépend du firmware déjà installé sur le clavier. Si vous avez un doute sur le firmware installé, consultez la [page générale des firmwares](installer-firmware.md)

### Si votre clavier utilise déjà un firmware QMK

Passez le clavier en mode bootloader, avec la combinaison de touches Fn + Echap (Fn + B pour le Dark Mage). Le clavier doit s'éteindre et ne plus être opérationnel.

Lancez l'outil de flash, et sélectionnez le type de puce "SN32F24x".
Dans la liste déroulante, le clavier doit être indiqué. Cliquez sur le bouton "Refresh" si nécessaire.
Modifiez le paramètre "QMK Offset" pour être à 0x00 s'il ne l'est pas déjà.

Cliquez sur le bouton "Flash QMK ...". Un explorateur de fichier s'ouvre, naviguez jusqu'au fichier BIN récupéré précédemment dans les pré-requis, puis sélectionnez-le.

L'outil de flash va installer le nouveau firmware. Ne touchez absolument pas le clavier tant que la barre de progression n'est pas terminée et que le mot "Finished" apparaît.

Le clavier redémarre de lui-même après l'installation.

### Si votre clavier utilise le firmware d'origine "Evision"

Lancez l'outil de flash, et sélectionnez le type de puce "SN32F24x".
Dans la liste déroulante, le clavier doit être indiqué. Cliquez sur le bouton "Refresh" si nécessaire.
Modifiez le paramètre "QMK Offset" pour être à 0x00 s'il ne l'est pas déjà.
Cliquez sur le bouton "Reboot to Bootloader [eVision]", attendez que la barre de progession se termine. Le clavier doit s'éteindre et ne plus être opérationnel.

Cliquez sur le bouton "Flash QMK ...". Un explorateur de fichier s'ouvre, naviguez jusqu'au fichier BIN récupéré précédemment dans les pré-requis, puis sélectionnez-le.

L'outil de flash va installer le nouveau firmware. Ne touchez absolument pas le clavier tant que la barre de progression n'est pas terminée et que le mot "Finished" apparaît.

Le clavier redémarre de lui-même après l'installation.

## Configurer QMK avec VIA

TODO
