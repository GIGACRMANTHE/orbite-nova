# ORBITE NOVA — version de travail 0.7.0
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
- F8 désactive/réactive NOVA. Le hangar constitue le menu principal, sans bouton de sortie.

## Encore à réaliser
Le HUD en partie conserve des composants issus d'ORBITE. Les lasers personnalisés partagent leur shader entre aperçu et partie ; leur échelle et leur luminosité dépendent aussi du rendu du jeu. Le catalogue de rochers sera ajouté séparément. Dépôt indépendant : GIGACRMANTHE/orbite-nova. Validation visuelle en navigateur et partie officielle nécessaire avant une diffusion générale.

## Validation
Tests locaux de démarrage, changement de thème, F8 et arrêt, progression persistante et dédoublonnage réussis. Ces tests ne valident pas le rendu WebGL réel.

Version 0.2.0 : fond cosmique 3840 px inclus, modèle officiel exposé via le catalogue disponible, flèches de coques et lasers, animation douce limitée à 30 images/s uniquement dans le hangar. Tests locaux du défilement circulaire, sélection, désactivation et arrêt réussis ; validation visuelle réelle à confirmer.

Version 0.3.0 : vaisseau droit sans oscillation angulaire automatique, commandes sociales du bas masquées, panneau autour de Jouer transparent. Six nouvelles coques et six tirs personnalisés avec shader commun au hangar et à la partie. Aperçu Original neutre. Validation visuelle réelle encore nécessaire.

Version 0.4.0 : nouvelles coordonnées de texture sur chaque face de la coque, matériaux indépendants des bases officielles, relief géométrique (96 pièces maximum par coque) et reflets d’environnement. Caméra orbitale avec vue frontale inclinée, rotation par glissement, rotation automatique facultative et retour à la vue initiale. Les collisions et règles officielles restent identiques.

Validation 0.4.0 : 198 combinaisons (33 modèles × 6 skins) contrôlées pour couverture, coordonnées valides, absence de reconstruction par image et restauration native. Six matériaux rendus avec le moteur Three.js r85 en aperçu local, sans erreur WebGL capturée. Pas encore validé dans une partie officielle. Le relief ajoute un objet de rendu par vaisseau ; les performances dépendent du matériel et du nombre de vaisseaux.

Version 0.5.0 : retrait des petites pièces répétées. 33 profils de modèles distincts règlent les chemins d’énergie, les voiles latéraux et les auras de coque. Les chemins sont posés sur la géométrie du modèle et coupés dans les espaces vides. Les voiles sont des ajouts visuels énergétiques, sans changement des collisions. Couleurs liées au matériau sélectionné ; animations partagées entre hangar et partie. Géométries des effets mises en cache par modèle, deux objets de rendu supplémentaires par coque. Les modèles inconnus utilisent un flux discret sans ailerons.

Contrôles : 198 combinaisons modèle/matériau et restauration native, aperçu local de six modèles officiels avec animations sans erreurs WebGL. Pas de validation en partie officielle à ce stade.

Version 0.6.0 : finition brossée et nuances nacrées, reflets rééquilibrés. Chargement avec miniature animée du vaisseau et progression native. Panneau de vol compact : modèle actuel, bouclier/capacité, énergie/capacité, score et kills du joueur local. Aucune valeur simulée dans le client : panneau masqué en cas de données absentes ou périmées, de mort ou de désactivation. La miniature est recalculée seulement au changement de modèle ou de matériau. Le panneau complète les informations natives.

Validation : aperçu local du chargement et du panneau avec données fictives explicitement signalées ; tests du raccordement aux champs natifs, bouclier nul, mort, données périmées, F8 et restauration des fonctions. Tests des 198 variantes de coques et du démarrage. Une vérification dans une partie officielle reste nécessaire.

Version 0.7.0 : hangar permanent avec Vaisseaux, Lasers, ECP et Ambiance. Les vrais contrôles ECP, matériaux et tirs sont intégrés lorsque présents, sans contourner les droits du compte. Respawn centré et allégé. Vaisseau et jauges de bouclier/énergie sur fond transparent en bas au centre : les jauges natives sont masquées uniquement quand leur remplacement dispose de valeurs valides, puis restaurées à la désactivation ou en cas de perte des données.

Sur ordinateur (largeur ≥ 850 px), classement à gauche, arsenal à droite, RCS en haut à gauche et chat en bas à gauche ; adaptation commune des coordonnées visuelles et cliquables. La disposition mobile native et le radar sont conservés. Le score natif, les cristaux et les vies restent disponibles. Validation : tests locaux des jauges, restauration, coordonnées HUD, démarrage ; aperçu local du hangar, ECP et respawn. Tests en partie officielle encore nécessaires.
