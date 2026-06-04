# Éditeur d’images local — Mini Paint avancé

## Présentation

Cet outil est un éditeur d’images local, inspiré de Paint, conçu pour permettre à un utilisateur de créer, composer, modifier et exporter une image directement depuis son navigateur.

L’application fonctionne entièrement côté client : les images importées restent sur l’ordinateur de l’utilisateur et ne sont pas envoyées vers un serveur. Elle peut donc être utilisée comme un outil simple, rapide et autonome pour manipuler des visuels, préparer des signatures, assembler des logos, annoter des captures ou créer des compositions graphiques légères.

## Objectif du projet

Le but du logiciel est de proposer un **nouveau Paint local**, plus adapté aux besoins courants de composition d’images :

- ajouter plusieurs images sur un même canevas ;
- déplacer et redimensionner librement les éléments ;
- travailler avec des calques ;
- recadrer l’image finale pour supprimer les zones blanches inutiles ;
- exporter dans une taille précise ;
- ajouter un filigrane si nécessaire ;
- rester simple à utiliser, sans installation lourde.

L’outil est pensé pour des usages pratiques comme :

- créer une image regroupant un logo et une signature ;
- préparer une bannière ou une image de communication ;
- annoter une capture d’écran ;
- redimensionner une image avant envoi ;
- fusionner plusieurs éléments graphiques dans un seul fichier ;
- produire rapidement une image finale propre au format PNG, JPEG ou WebP.

## Fonctionnement local

L’application est fournie sous la forme d’un fichier HTML autonome.

Il suffit d’ouvrir le fichier dans un navigateur moderne pour l’utiliser.

Aucune installation serveur n’est nécessaire.

Les traitements sont réalisés dans le navigateur grâce à HTML, CSS et JavaScript.

## Fonctionnalités principales

### Canevas de travail

- Canevas blanc de base.
- Taille du canevas modifiable.
- Zone de travail scrollable si le canevas dépasse la fenêtre.
- Zoom interne au canevas.
- Déplacement de la vue avec clic droit maintenu et glissement.
- `Ctrl + molette` pour zoomer ou dézoomer la zone de travail sans zoomer toute la page.

### Import d’images

- Import d’une ou plusieurs images.
- Glisser-déposer depuis un dossier.
- Coller une image depuis le presse-papiers avec `Ctrl + V`.
- Import possible de formats courants selon la compatibilité du navigateur :
  - PNG ;
  - JPG / JPEG ;
  - SVG ;
  - BMP ;
  - WebP ;
  - GIF, généralement en image fixe.

### Manipulation des éléments

Chaque image ou objet ajouté devient un élément manipulable :

- déplacement libre ;
- redimensionnement ;
- conservation des proportions ;
- rotation ;
- duplication ;
- suppression ;
- verrouillage ;
- affichage ou masquage ;
- changement d’ordre avant/arrière.

### Calques

L’éditeur permet de gérer les éléments sous forme de calques :

- liste des calques ;
- sélection d’un calque ;
- visibilité ;
- verrouillage ;
- réorganisation ;
- suppression.

Cette logique facilite la composition d’images complexes, par exemple avec un logo, une signature, du texte et des formes.

### Outils de dessin

L’application intègre plusieurs outils inspirés de Paint :

- pinceau ;
- gomme ;
- ligne ;
- flèche ;
- rectangle ;
- ellipse ;
- texte ;
- pipette ;
- sélection ;
- recadrage.

### Recadrage

Deux types de recadrage sont disponibles :

#### Recadrage d’un élément

Permet de recadrer une image ou une zone sélectionnée.

#### Recadrage du canevas

Permet de supprimer automatiquement les zones blanches inutiles autour du contenu visible.

Cette fonction est particulièrement utile avant l’export final afin d’éviter une image trop grande avec beaucoup de marge blanche.

### Redimensionnement d’export

Avant de télécharger l’image finale, l’utilisateur peut choisir la taille de sortie :

- largeur d’export ;
- hauteur d’export ;
- conservation automatique des proportions du canevas.

Le canevas de travail ne change pas : seule l’image exportée est redimensionnée.

### Filtres et ajustements

Des réglages simples peuvent être appliqués aux images :

- luminosité ;
- contraste ;
- saturation ;
- noir et blanc ;
- flou.

### Filigrane

L’éditeur propose une option de filigrane à l’export :

- activation ou désactivation ;
- texte du filigrane ;
- opacité ;
- application uniquement au fichier exporté.

Le filigrane ne modifie pas le canevas de travail pendant l’édition.

### Export

L’image finale peut être exportée dans plusieurs formats :

- PNG ;
- JPEG ;
- WebP.

L’export prend en compte :

- la composition finale ;
- les calques visibles ;
- la taille d’export choisie ;
- le recadrage éventuel ;
- le filigrane si activé.

### Sauvegarde du projet

L’éditeur permet de sauvegarder et recharger un projet au format JSON afin de reprendre une composition plus tard.

## Cas d’usage typiques

### Fusionner un logo et une signature

1. Ouvrir l’éditeur.
2. Ajouter le logo de l’entreprise.
3. Ajouter la signature de l’agent.
4. Déplacer les deux images librement.
5. Ajuster leur taille.
6. Recadrer le canevas pour supprimer les marges blanches.
7. Choisir la taille d’export.
8. Télécharger l’image finale.

### Préparer une image pour un document

1. Importer une image.
2. Redimensionner ou recadrer.
3. Ajouter du texte ou une flèche.
4. Exporter au format PNG ou JPEG.

### Annoter une capture d’écran

1. Coller ou importer une capture.
2. Ajouter des formes, flèches ou textes.
3. Recadrer le canevas.
4. Exporter l’image annotée.

## Avantages

- Fonctionne localement.
- Ne nécessite pas de compte utilisateur.
- Ne nécessite pas d’installation complexe.
- Respecte la confidentialité des images.
- Simple à déployer : un fichier HTML suffit.
- Interface proche d’un outil de dessin classique.
- Adapté aux besoins rapides de composition et d’export.

## Limites connues

- Les performances dépendent du navigateur et de la taille des images.
- Les GIF animés sont généralement traités comme une image fixe.
- Certains SVG complexes peuvent dépendre des capacités du navigateur.
- L’outil n’a pas vocation à remplacer un logiciel professionnel comme Photoshop, GIMP ou Illustrator.
- Il vise plutôt un usage simple, rapide et local, dans l’esprit d’un Paint amélioré.

## Installation

Aucune installation particulière n’est nécessaire.

Télécharger le fichier HTML de l’éditeur, puis l’ouvrir dans un navigateur récent :

- Google Chrome ;
- Microsoft Edge ;
- Mozilla Firefox ;
- Safari, selon compatibilité.

## Utilisation

1. Ouvrir le fichier HTML.
2. Ajouter une ou plusieurs images.
3. Modifier la composition sur le canevas.
4. Utiliser les outils de dessin, texte ou recadrage.
5. Choisir la taille d’export.
6. Télécharger l’image finale.

## Confidentialité

L’application fonctionne côté navigateur.

Les images sont chargées et traitées localement sur le poste de l’utilisateur.

Aucun transfert vers un serveur n’est nécessaire pour les fonctionnalités principales.

## Vision du projet

Ce projet a pour ambition de devenir un **Paint local modernisé** :

- plus flexible que Paint pour composer plusieurs images ;
- plus simple qu’un logiciel de graphisme professionnel ;
- adapté à des usages administratifs, bureautiques et quotidiens ;
- utilisable immédiatement depuis un navigateur.

L’objectif est de fournir un outil pratique, accessible et autonome pour travailler rapidement des images sans dépendre d’un service en ligne.
