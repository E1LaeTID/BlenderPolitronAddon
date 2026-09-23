# Politron Builder for Blender

**Politron Builder** est un add-on Blender qui génère en un clic des **géométries complexes avec un nombre limité de sommets**. Les formes, appelées ici *politrons*, sont construites par extension dimensionnelle de polygones, selon une démarche comparable à la construction et à la projection de polytopes.

> English summary: a Blender add-on that generates low-vertex complex geometry from polygon-based dimensional extensions, useful for blocking, experimentation and Boolean modeling.

## Qu'est-ce qu'un politron ?

Dans ce projet, un politron est une géométrie dérivée d'un polygone de base puis étendue à travers des relations dimensionnelles supplémentaires. L'objectif n'est pas de représenter directement un objet mathématique complet de dimension supérieure, mais d'obtenir dans Blender une géométrie exploitable issue de cette démarche.

Certaines structures correspondent à une projection statique assimilée à une construction 4D. D'autres nécessitent une animation ou une succession d'états pour communiquer une extension assimilée à une construction 5D. Une seule vue fixe ne suffit donc pas toujours à révéler leur organisation.

## À quoi sert l'outil ?

- générer rapidement des volumes inhabituels ;
- obtenir une base complexe avec relativement peu de sommets ;
- accélérer la phase de blocking ;
- créer des opérandes pour des booléens ;
- étudier des variations construites à partir de différents polygones ;
- explorer visuellement des principes d'extension dimensionnelle.

## Installation

1. Téléchargez le dépôt au format ZIP.
2. Dans Blender, ouvrez **Edit > Preferences > Add-ons**.
3. Choisissez **Install from Disk**.
4. Sélectionnez l'archive et activez l'add-on.
5. Ouvrez le panneau de l'outil dans la vue 3D.

## Utilisation rapide

1. Ouvrez le panneau Politron Builder.
2. Réglez la dimension ou la longueur de référence.
3. Choisissez le polygone de base.
4. Cliquez sur **Generate**.
5. Inspectez la forme sous plusieurs angles.
6. Utilisez-la comme volume autonome, base de blocking ou opérande booléen.

## Pourquoi peu de sommets ?

Le générateur cherche à produire la structure complexe dès la construction initiale, plutôt que de dépendre uniquement de subdivisions successives. Le nombre exact de sommets varie avec le polygone et le type de politron généré.

## Limites connues

- Toutes les bases polygonales ne produisent pas nécessairement le même niveau de finition.
- Certaines options expérimentales peuvent afficher un message dans la console au lieu de générer une forme complète.
- Une projection 4D ou une évolution 5D reste une représentation dans l'espace 3D de Blender.
- Les formes doivent être contrôlées avant impression 3D ou utilisation dans une opération booléenne.
- Le comportement peut varier selon la version de Blender et la complexité de la scène.

## Questions fréquentes

### Qu'est-ce qu'une géométrie 4D dans Blender ?

Blender affiche un espace 3D. Le terme désigne ici une géométrie résultant d'une construction ou projection inspirée d'une extension dimensionnelle, et non l'affichage direct d'un espace à quatre dimensions.

### Pourquoi certaines structures doivent-elles être animées ?

Une succession d'états peut révéler des relations qui restent ambiguës dans une projection statique. L'animation sert alors de support de lecture pour les constructions assimilées à une extension 5D.

### L'outil sert-il uniquement à produire des objets mathématiques ?

Non. Les formes peuvent être utilisées comme bases artistiques, volumes de blocking, objets décoratifs ou opérandes pour la modélisation booléenne.

### Peut-on utiliser un politron pour l'impression 3D ?

Oui après vérification : contrôlez les normales, les intersections, l'étanchéité du maillage, son échelle et les contraintes de votre procédé d'impression.

### Quelle différence avec Fractal Addon ?

Politron Builder produit une géométrie complexe à partir d'une extension polygonale. Fractal Addon répète récursivement une structure issue d'une coupole de Johnson modifiée.

### Où trouver tous les générateurs dans un seul projet ?

[CoTQoQ Builder](https://github.com/E1LaeTID/CoTQoQ_builder) réunit les quatre outils Blender.

## Apprendre Blender

Une [formation Blender destinée aux débutants](https://www.udemy.com/course/modelisation-impression-3d-avec-blender-tous-niveaux/?couponCode=LETSLEARNNOW) permet d'aborder plus simplement les bases de la modélisation et de l'impression 3D avant de modifier manuellement les géométries générées.

## Écosystème

- [CoTQoQ Builder](https://github.com/E1LaeTID/CoTQoQ_builder)
- [3D Tool Helper](https://github.com/E1LaeTID/3DToolHelperForBlender)
- [Maze Builder](https://github.com/E1LaeTID/BlenderMazeBuilderAddon)
- [Fractal Addon](https://github.com/E1LaeTID/BlenderFractalAddon)
- [Portail E1LaeTID](https://e1laetid.github.io/)

## Statut et licence

Prototype fonctionnel et expérimental. Le code est distribué sous **Apache License 2.0** ; consultez le fichier [LICENSE](LICENSE).
