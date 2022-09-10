# med-planification
Mesure des étoiles doubles - planification

## Introduction

Quelques notes concernant le vocabulaire utilisé dans ce repo.

* WDS : le Washington Doubles Star Catalog.
* système : un système d'étoiles doubles (ou multiples) selon la désignation de découvreur du WDS (Discoverer & Number); par ex. STTA 254 ou STF 60.

## Dossier LISTES

Contient les listes dans diver format (PDF, txt, HTML, etc). La source de la liste peut-être déduite selon la nomenclature suivante :
* astrodm_...* : liste provenant d'un des modules de la librairie astrodm créée par Dominique Martel.

## Dossier LOTS
Les fichiers de ce dossier sont au format __LibreOffice ods__ (feuille de calcul).

Ils sont exploités avec un script Python (__cree_systeme_beta03.py__) qui lit le lot et crée les dossiers correspondant à chaque système présent dans la liste.

## Exemple de tableau de planification<br>
|système |Date prévue|Session|
|--------|-----------|-------|
|SFT 60  |2022-09-16 |1      |
|STTA 254|2022-09-16 |2      |

Cette image a été collée à partir du Presse-papier.<br><br>
![image2](https://user-images.githubusercontent.com/52057610/189502393-4bbe468b-7a19-4b2b-9824-7b253af39a5d.jpg)

#### Distance angulaire (en arcsec) du maxima d'ordre n d'un patron de diffraction créé par un masque à fente
$$z = 206264.806 " \frac{n \lambda}{Lf + Df}$$...(1)<br><br>
où :

$z$ est la séparation angulaire du maxima d'ordre n (arcsec)

__206264.806__ est le nombre de secondes d'arc dans un radian

$n$ = 1 pour les maxima de 1er ordre

$\lambda$ est la longueur d'onde de la lumière en mm

$Lf$ est la largeur des fentes en mm

$Df$ est l'espacement des fentes, c.-à-d. la largeur des bandes opaques entre les fentes en mm
