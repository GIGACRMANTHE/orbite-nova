# ORBITE full edition — version 0.9.5
Créateur : GIGACRMANTHE.

## Installation
[Installer NOVA directement](https://raw.githubusercontent.com/GIGACRMANTHE/orbite-nova/main/ORBITE-NOVA.user.js), puis cliquer sur Installer dans Tampermonkey. Désactiver ORBITE Light et les autres clients Starblast avant de recharger https://starblast.io/. NOVA dispose de ses propres préférences et de son propre nom ; le dépôt ORBITE Light n'a pas été modifié.

## Inclus
- Hangar holographique sur fond cosmique fourni par le créateur ; onglets Vaisseaux et Lasers, navigation par flèches et molette. Bouton Jouer et modes officiels sous l’aperçu.
- Aperçu 3D du modèle officiel, rotation par glissement, défilement molette, recentrage et anneaux de projection.
- Onze coques et six tirs personnalisés, avec option Original. Le modèle d'exposition n'accorde pas un vaisseau de départ différent en partie officielle.
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

Version 0.9.2 : annulation des déplacements 0.7 du classement, RCS, arsenal et chat ; positions officielles conservées. Statistiques compactes en haut à gauche. Remplacement des éléments natifs disponibles (bouclier, énergie, cristaux, score, niveau, vies), avec restauration si données absentes ; le réticule natif reste intact. Suppression des anneaux de projection du hangar. Radar à fond radial sombre et repères fins, contacts et informations natifs conservés.

Studio ECP : aperçu agrandi, import local PNG/JPEG/WebP jusqu’à 8 Mo et 8192 px, recadrage carré centré en 512 px, sauvegarde sur cet appareil, bouton d’effacement. L’image remplit l’intérieur de l’ECP sans changer ses droits ni être envoyée aux autres joueurs.

Cinq matériaux supplémentaires : Cosmos profond (étoiles et parallaxe), Verre prismatique (transparence et reflets simulés), Couronne ionique, Brume spectrale (coque déformée visuellement et voile animé), Céramique mate sans aura. Ces effets ne sont pas une simulation volumétrique de fumée ni une réfraction physique du décor.

Validation 0.8 : 363 combinaisons modèle/matériau, démarrage, restauration des jauges ; import d’image et rendu des matériaux vérifiés dans l’aperçu local. Partie officielle et agencement sur toutes les résolutions restent à vérifier.


## Version 0.9.2

- Hangar à miniatures : coques, lasers et insignes, puis grand aperçu orientable.
- ECP reconstruit avec le dessinateur natif et ses proportions ; son image reste un dessin sur une surface 3D orientable. Import PNG/JPG/WebP local, plus Astrarium, Sceau fractal et Soleil noir.
- Quatre anciens matériaux retirés : Verre stellaire, Titane polaire, Céramique solaire et Porcelaine orbitale.
- Galerie des fonds : la sélection utilise le même univers dans le menu et en partie.
- Pseudo : champ officiel conservé, envoyé normalement par le jeu ; les personnalisations visuelles restent locales.
- Réglages : bouton du hangar relié à la fenêtre officielle, avec nouvelle présentation.
- Un seul panneau de chargement visible ; statistiques transparentes plus lisibles, bouclier faible signalé en couleur.

Tests : 231 couples modèle/matériau, shaders des six tirs, restauration des statistiques natives, démarrage sans serveur, arrêt/F8. Aperçu navigateur avec données fictives validé pour ECP, fonds et chargement. Pas de validation multijoueur réelle ni garantie de compatibilité avec toutes les futures versions de Starblast.


## Correctif 0.9.2

- Détection de la coque par sa géométrie, y compris lorsque le nom du matériau est obfusqué par le jeu. Les aperçus utilisent un atelier isolé et libèrent leurs modèles temporaires.
- Miniatures calculées au maximum une fois toutes les 100 ms, puis conservées en cache. Suppression de rafraîchissements doublons ; découverte des composants et balayages espacés.
- Cache ECP du classement renouvelé lors des changements ; transformation du dessin réinitialisée avant application du motif. Les insignes restent une personnalisation visible uniquement sur cet appareil.
- Panneau repliable en partie : E (emote vide), C (phrase de 5 emotes), F8, activation/désactivation. Le bouton reste disponible lorsque le client est désactivé.

Validation : tests des 231 couples avec les propriétés obfusquées du jeu, cache ECP, shaders, statistiques, démarrage et F8. Aperçus et panneau testés dans une simulation locale. Pas de mesure FPS ni de validation du classement dans une partie réelle.


## Correctif 0.9.2 — aperçu indépendant

Le registre du jeu est une variable interne, pas nécessairement une propriété de window. Le hangar embarque désormais les géométries exportées des 33 modèles officiels ; il ne construit plus de vaisseaux avec le moteur natif pour les aperçus. Le rendu en partie continue d’utiliser les modèles du jeu. L’option Original a un aperçu neutre dans le hangar.

Miniatures limitées aux éléments visibles, cache borné, tentatives de rendu espacées puis arrêtées après trois échecs. Protection contre le démarrage d’une seconde copie du client.

Vérification navigateur : aperçu principal et miniatures visibles sans registre ni constructeur de vaisseau du jeu. Validation en partie réelle et mesure des freezes non effectuées.

## 0.9.3
Préparation progressive des coques et lasers du hangar, cache de géométries et miniatures dans un rendu séparé. En partie, les couches supplémentaires de géométrie sont retirées et les shaders de profondeur utilisent deux couches au lieu de quatre ; les matériaux personnalisés restent actifs. Pseudo et aperçu ECP recentrés. Les performances en combat réel restent à mesurer.

Les réacteurs en partie conservent leurs jets colorés, avec une géométrie allégée et sans nuage de particules supplémentaire. La recherche des tuyères est espacée à 500 ms.

## 0.9.4
- Sélections : aucune reconstruction globale du moteur au changement de coque ou ECP, cache des reflets partagé, miniatures ECP en 2D et invalidation par image. Les mises à jour natives ECP sont réparties sur plusieurs images.
- Coques : Opale vivante, Abîme gravitationnel, Mercure irisé.
- HUD compact : Placer les UI, glisser les zones encadrées, Terminer. Positions enregistrées localement ; bouton de réinitialisation. Classement, RCS, munitions, emotes et radar sont déplacés via leurs rectangles natifs quand ils sont détectés.
- Statistiques : barre des cristaux et score lu depuis le même joueur que le compteur officiel.
- Validation : tests automatisés, aperçu local des sélections, shaders et glisser-déposer. Pas de mesure de fluidité dans une partie publique peuplée.

## 0.9.5
Les panneaux du jeu retrouvent leurs positions et dimensions officielles. Les anciennes positions HUD sont ignorées. Un seul bouton ORBITE discret rassemble emotes, raccourcis et activation. Glisser ce bouton pour le déplacer ; cliquer pour ouvrir. Sa position seule est enregistrée.

Le panneau personnalisé ne contient plus score/kills ni niveau/vies. Le compteur officiel du score est conservé.
