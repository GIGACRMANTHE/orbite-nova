# ORBITE NOVA — version de travail 0.4.0
Créateur : GIGACRMANTHE.

## Installation
[Installer NOVA directement](https://raw.githubusercontent.com/GIGACRMANTHE/orbite-nova/main/ORBITE-NOVA.user.js), puis cliquer sur Installer dans Tampermonkey. Désactiver ORBITE Light et les autres clients Starblast avant de recharger https://starblast.io/. NOVA dispose de ses propres préférences et de son propre nom ; le dépôt ORBITE Light n'a pas été modifié.

## Inclus
- Hangar holographique sur fond cosmique fourni par le créateur ; onglets Vaisseaux et Lasers, navigation par flèches et molette. Bouton Jouer et modes officiels sous l’aperçu.
- Aperçu 3D du modèle officiel, rotation par glissement, défilement molette, recentrage et anneaux de projection.
- Six nouvelles coques et six tirs personnalisés, avec option Original. Le modèle d'exposition n'accorde pas un vaisseau de départ différent en partie officielle.
- Nouveaux styles de chargement et de retour au combat ; actions et délais officiels conservés.
- Progression locale : 100 XP/kill, 1 XP/100 points (plafond 1000), 500 XP/victoire. Attribution à la fin de partie uniquement si le jeu expose ses résultats. Pas de crédit pour une partie quittée sans résultat. Niveau de progression, pas estimation de compétence. Données propres à ce navigateur, sans serveur.
- Fonds et assets inclus ; aucun import manuel.
- F8 restaure les modifications ; bouton Menu classique ferme le hangar ; bouton Hangar NOVA le rouvre.

## Encore à réaliser
Le HUD en partie conserve des composants issus d'ORBITE. Les lasers personnalisés partagent leur shader entre aperçu et partie ; leur échelle et leur luminosité dépendent aussi du rendu du jeu. Le catalogue de rochers sera ajouté séparément. Dépôt indépendant : GIGACRMANTHE/orbite-nova. Validation visuelle en navigateur et partie officielle nécessaire avant une diffusion générale.

## Validation
Tests locaux de démarrage, changement de thème, F8 et arrêt, progression persistante et dédoublonnage réussis. Ces tests ne valident pas le rendu WebGL réel.

Version 0.2.0 : fond cosmique 3840 px inclus, modèle officiel exposé via le catalogue disponible, flèches de coques et lasers, animation douce limitée à 30 images/s uniquement dans le hangar. Tests locaux du défilement circulaire, sélection, désactivation et arrêt réussis ; validation visuelle réelle à confirmer.

Version 0.3.0 : vaisseau droit sans oscillation angulaire automatique, commandes sociales du bas masquées, panneau autour de Jouer transparent. Six nouvelles coques et six tirs personnalisés avec shader commun au hangar et à la partie. Aperçu Original neutre. Validation visuelle réelle encore nécessaire.

Version 0.4.0 : nouvelles coordonnées de texture sur chaque face de la coque, matériaux indépendants des bases officielles, relief géométrique (96 pièces maximum par coque) et reflets d’environnement. Caméra orbitale avec vue frontale inclinée, rotation par glissement, rotation automatique facultative et retour à la vue initiale. Les collisions et règles officielles restent identiques.

Validation 0.4.0 : 198 combinaisons (33 modèles × 6 skins) contrôlées pour couverture, coordonnées valides, absence de reconstruction par image et restauration native. Six matériaux rendus avec le moteur Three.js r85 en aperçu local, sans erreur WebGL capturée. Pas encore validé dans une partie officielle. Le relief ajoute un objet de rendu par vaisseau ; les performances dépendent du matériel et du nombre de vaisseaux.
