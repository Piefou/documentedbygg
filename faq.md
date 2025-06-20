# Foire aux questions

Est-ce que les claviers sont compatibles Mac/Linux ?

Quels sont les raccourcis présents sur les claviers ?

Peux t-on synchroniser le RGB selon les logiciels/jeux lancés ?
SignalRGB

Est-ce que les claviers sont sans-fil ?
Non. L'idée de proposer des versions sans-fil est étudiée, mais nécessite de la réflexion pour proposer une implémentation propre et fonctionnelle.

Quels keycaps/switchs/stabilisateurs puis-je mettre sur le clavier ?
Tous les keycaps et switchs au format MX standard peuvent être mis sur les claviers.
Pour les modèles n'acceptant que les switchs 3-pins, il est possible de couper les pins plastiques des switchs 5-pins pour les y mettre.
Seuls les stabilisateurs à fixer sur le PCB peuvent être installés.
Les switchs low-profile ne sont pas compatibles avec les claviers.

Quels sont les dimensions des claviers ?
Vous pouvez trouver les dimensions et masse de chaque modèle sur la page récapitulative des produits [ici]
(Taille du câble USB)

Comment puis-je contacter DesignedByGG pour une demande ?
Page SAV

## Problèmes couramment rencontrés

Ma touche Windows ne fonctionne pas.
La combinaison Fn + Win permet d'activer/désactiver la touche Windows. Refaites cette combinaison pour réactiver la touche.

Le driver ne reconnaît plus mon clavier.
Le firmware installé n'est peut être pas compatible avec le driver. Suivez la procédure de réinstallation du firmware d'origine sur la page [ici].

VIA ne reconnaît plus mon clavier.
Chargez dans VIA le fichier JSON qui peut être trouvé [ici].
Le firmware installé n'est peut être pas compatible avec VIA. Suivez la procédure de réinstallation de QMK sur la page [ici].


## Fonctionnalités absentes

- Pas de fonctionnalités spécifiques HE : Rapid trigger, SOCD, Snap-tap, analogique ...
- Pas de gestion des profils de RGB. La fonctionnalité est présente dans le driver mais n'est pas fonctionnelle.

### Avec le firmware d'origine 

- Pas de personnalisation du layer (raccourcis en combinaison avec la touche Fn)

### Avec le firmware QMK :

- Pas de réglage touche par touche du RGB.


## Roadmap au 20/06/2025

### En cours de production

- "Red Blade 75", version 75% du Red Blade, avec la même fiche technique, seul le layout change
- Nouvelle suite logicielle, avec firmware maison, et nouveau driver avec compatibilité QMK/json-VIA

### En cours de prototypage

- Casque audio avec planars
