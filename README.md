# med-planification
Mesure des étoiles doubles - planification

## Introduction
Ce repo contient les listes servant à la planifications de mes observations d'étoiles doubles. Il ne contient aucune données d'acquisition et les scripts en langage Python qui servent à exécuter les opérations de collecte des données présentées dans les listes ne se trouvent pas dans ce repo (librairie astrodm de l'auteur).

## Lexique

Quelques notes concernant le vocabulaire utilisé dans ce repo.

* WDS : le Washington Doubles Star Catalog.
* système : un système d'étoiles doubles (ou multiples) selon la désignation de découvreur du WDS (Discoverer & Number); par ex. STTA 254 ou STF 60.

## Utilisation
### Dossier LISTES
Au fur et à mesure des activités (planification, repérage, acquisition des données, pré-réduction et post-réduction), le suivi est effectué à l'aide des scripts de la librairie __astrodm__. Certains de ces scripts colligent les données qui se trouvent dans la structure de répertoires située dans les dossiers de données (en local sur l'ordinateur de l'auteur). Ce sont ces données sont présentées sous forme de listes au format texte.

Les listes se trouvent dans le dossier LISTES. Dans ce dossier, la nomenclature des listes est la suivante :<br>
(Note : la date d'exécution de la liste est indiquée à la fin du nom de fichier)
* __astrodm-liste-info-systemes-trie(id_system+const)-2022-09-11T143528.txt__ : liste le contenu de tous les fichiers « _info_système.csv » présents dans la structure, ici triés par id_system et const.
* __astrodm-liste-prog-obs-trie(id_system+obs_prog)-2022-09-11T143444.txt__ : liste des programmes d'observation, ici triés par id_system et obs_prog.
* __astrodm_table_resultats_mesures.html__ : table de l'ensemble des mesures réalisées.

### Dossier LOTS
Les fichiers de ce dossier sont au format __LibreOffice ods__ (feuille de calcul).

Ils sont exploités avec un script Python (__cree_systeme_beta03.py__) qui lit le lot et crée les dossiers correspondant à chaque système présent dans la liste.
