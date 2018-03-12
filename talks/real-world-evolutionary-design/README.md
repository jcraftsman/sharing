# Real world evolutionary design

## Format

Hands-on workshop (2h - 3h)

## Pitch

Tu veux construire une application, en gardant une boucle de feedback rapide tout au long du développement&nbsp;?

Tu veux avoir une application souple, sans finir par dessiner des diagrammes ou écrire un DAT qui sera obsolète avant le début du développement&nbsp;?

Tu arrives à anticiper plusieurs besoins non fonctionnels (dispo, perf...), mais tu ne sais pas par quoi commencer&nbsp;?

Tu trouves les katas pour TDD et clean code rigolos mais trop simples par rapport aux vrais problèmes de la vraie vie&nbsp;?

Ce workshop est taillé pour toi&nbsp;!

L'objectif de ce workshop est de construire une application qui intéragit avec des services externes (AWS S3 et une web api).

Nous allons faire de l'_Outside-in TDD by wishful thinking_. Cette variante de TDD favorise un design émergeant tout en restant focalisé sur la valeur à livrer.

## Motivation et plan

Durant ce workshop, nous allons réaliser une user story qui permettra à l'utilisateur de rechercher une image en fonction d'une information qu'elle contient.
Pour cela, nous allons développer un module qui analysera le contenu des images depuis un bucket S3. Ce contenu sera notifié à une web app via une api REST.

Voici le déroulement :

- Les participants vont cloner un repo et lancer un script qui leur permettra d'installer les outils dont ils auront besoin (10 min)
- Je ferai une présentation pour introduire les concepts que nous allons voir durant le workshop (30 min)
- J'annoncerai l'objectif et les contraintes de l'itération 1 (5 min)
- Itération 1 (30 min)
- Débrief de l'itération 1 (5 min)
- Pause (10 min)
- J'annoncerai l'objectif et les contraintes de l'itération 2 (5 min)
- Itération 2 (30 min)
- Débrief de l'itération 2 (5 min)
- J'annoncerai l'objectif et les contraintes de l'itération 3 (5 min)
- Itération 3 (30 min)
- Conclusion (15 min)

Au début de chaque itération, les participants auront le choix de continuer sur leur version de code ou de démarrer depuis une version du repo qui contient tous les prérerequis de l'itération à suivre.

En suivant une approche outside-in, nous allons guider les développements par l'usage. Nous allons nous concenctrer à coder juste ce qu'il faut pour réaliser l'user story pour réduire toute complexité accidentelle.

Les règles d'implémentation "by wishful thinking" vont nous aider à faire émerger un design plus souple et isoler l'infra du domaine (évitant ainsi les piège OO : rigidité, fragilité, immobilité).

Une fois qu'une version fonctionnelle sera réalisée, nous essaierons d'introduire des besoins de perf. En ayant séparé les préoccupations au préalable, nous verrons comment il sera simple de les satisfaire.
