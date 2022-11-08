Formation : analyse spatiale des agroécosystèmes avec R

CONTEXTE
Cette formation s’est déroulée sur 3 jours (19h00) en présentiel à l’UMR SAS les 31 Août, 7 Septembre et 10 Septembre 2021. Elle a été financée par l’UMR SAS et réalisée dans le cadre de la formation interne des agents de l’UMR SAS.
Le public visé est des personnes ayant des bases en R et/ou des compétences avancées dans un autre langage de programmation et/ou des connaissances en SIG, ET avec un intérêt pour le traitement automatisé de données spatialisées, via le langage de programmation R.
De par son format, cette formation est adaptée à l’autoformation. Le nombre d’heures nécessaires pour l’effectuer pouvant varier selon votre familiarité avec R et vos compétences en programmation/SIG.
Sept modules ont été dispensés, dont deux modules (2 et 3) n’étant pas propres à l’analyse de données spatiales : 
1.	Introduction : Motivations et exemples (1h)
2.	Manipulation de données avec le tidyverse (1h30)
3.	Les bases de ggplot (1h)
4.	Analyse de données vectorielles géolocalisées avec le package sf (Partie 1 et 2, 7h30)
5.	Analyse de données raster avec le package raster (4h)
6.	Délimitation de bassins versants et analyse de terrain avec le package whitebox (2h00)
7.	Cartographie thématique avec ggplot et tmap (2h)

Organisation de la formation : Blandine Lemercier, UMR SAS
Liaison avec la formation interne INRAE : Nouraya Akkal-Corfini, UMR SAS
Réalisation de la formation : Antoine Casquin, UMR SAS
 
CONTENU DETAILLE DE LA FORMATION
1.	Introduction : Motivations et exemples (1h)
1.1.	Intérêt d’un flux de travail automatisé
1.2.	Accès aux packages métiers et APIs
1.3.	Galerie de cartes réalisées en R
2.	Manipulation de données avec le tidyverse (1h30)
2.1.	Chargement de .csv
2.2.	Manipulation de données via les verbes du package dplyr : select, filter, mutate, group_by, summarise …
2.3.	Utilisation du « pipe » pour enchainer les traitements sur les données
2.4.	Exercices et corrections sur des données multi-sites / multi-dates de qualité de l’eau
3.	Bases de ggplot2 (1h)
3.1.	Montage d'un ggplot : exemples pas à pas (« points », « lignes », « facettes », « tuiles » …)
3.2.	Exercices et corrections sur des données multi-sites / multi-dates de qualité de l’eau
4.	sf : LE package pour le traitement et l’analyse de données vectorielles géolocalisées en R (7h30)
4.1.	Partie 1
4.1.1.	 Fonctionnement du package sf
4.1.2.	 Chargement de données spatialisées et structure d’un objet sfc
4.1.3.	 Systèmes de coordonnées
4.1.4.	 Visualisation rapide (plot, tmap et ggplot)
4.1.5.	 Opérations sur les attributs
4.1.6.	 Opérations spatiales de type « confirmation » : contains, touches, is_within, is_within_distance …
4.1.7.	 Exercices en deux parties : Sélection par attribut et relations spatiales simples (4_1, basé sur la BD Carto) et Imbrications multiples (4_2, basé sur la délimitation des BV bretons)
4.2.	Partie 2
4.2.1.	 Transformations et projections
4.2.2.	 Calcul d’aires et de longueurs
4.2.3.	 Opérations spatiales : Recadrage, Buffer, Intersection, Union, Agrégation …
4.2.4.	 Inversion de coordonnées
4.2.5.	 Jointures sur les attributs
4.2.6.	 Jointures spatiales
4.2.7.	 Pour aller plus loin
4.2.8.	 Exercices et corrections : méthaniseurs et petites régions agricoles en Bretagne (4_3)
5.	Traitement et analyse de données raster avec {raster} (4h)
5.1.	Propriétés des rasters et visualisation rapide
5.2.	Extraction selon une emprise ou un masque
5.3.	Préparer un jeu de données raster pour l’analyse : projection, transformation, ré-échantillonage, « brique » de rasters
5.4.	Opérations sur les rasters : Reclassification, Opérations arithmétiques, Autres opérations
5.5.	Statistiques zonales
5.6.	Calculs sur des rasters ou bien des polygones ?
5.7.	Exercice
5.8.	Pour aller plus loin : {stars] et {terra}, le futur de l’analyse de raster en R. Lien vers un workshop {terrra] récent. 
6.	Analyse de terrain et délimitation de bassins versants avec {whitebox} (2h)
6.1.	Description du package whitebox et alternatives
6.2.	Principes généraux de fonctionnement du package
6.3.	Délimitation de bassins versants : exemple de Naizin : préparation des données, recollage des points sur le réseau hydrographique, délimitation « par lot », conversion en polygones
6.4.	Calcul d'indices topographique avec whitebox : pente, orientation, courbure …
6.5.	Calcul d’indices topographiques pour n BVs : initialisation et boucle (distances à l’exutoire, distances à l’hydrographie, flux accumulés sur les versants …)
7.	Cartographie thématique avec R : exemples avec ggplot2 et tmap (2h)
7.1.	Echelles de couleurs (catégorielle, séquentielle, divergente)
7.2.	Planche avec plusieurs cartes/variables : méthode « facet_wrap » et méthode « patchwork » (ggplot2)
7.3.	Ajouter des éléments cartographiques avec le package ggspatial
7.4.	Exemples vectoriel et raster avec le package tmap, export « figure » et export web.

MATERIEL PEDAGOGIQUE
Le dossier de la formation contient ce Lisez-moi à la racine et quatre sous-dossiers : cheat-sheet, exercice, installation, et slide.
Installation du poste de travail
Dans le dossier installation, deux fichiers sont présents : Configuration du poste de travail – Rspatial.docx qui est un tutoriel pour mettre à jour R et un script install_packages.R qui installe automatiquement les packages utilisés au long de la formation.
Slides
Des slides comprenant une partie théorique courte et de nombreux exemples de codes commentés sont disponibles pour chaque module (sauf le 7). Ces slides sont au format .html mais sont utilisables hors-ligne. Ils ont la particularité d’avoir été écrits en RMarkdown, avec le package xaringan. Les sources sont mises à disposition dans le sous dossier source. Pour les compiler, il est nécessaire d’installer quelques packages en plus (voir code source), et de copier le sous-dossier exercice/raw_data dans le sous-dossier slide/source.
Exercices
Pour les modules 2, 3, 4.1, 4.2 et 5, des exercices réalisables à partir du contenu des slides sont disponibles. A chacun de ces modules correspond un fichier xxx_Enonce.R et un fichier xxx_Correction.R. Les corrections sont très largement commentées et sont complémentaires des slides, il est recommandé de les lire même si vous n’avez pas rencontré de difficulté pour résoudre les exercices. Pour certaines questions, plusieurs manières de répondre à la question sont discutées. 
Les données se trouvent dans la un sous-dossier raw_data. Afin de réaliser facilement les exercices, il est conseillé de définir le répertoire de travail de R comme celui où se trouve le dossier exercice. Des sous-dossiers xxx_output vides servent à l’export des résultats pour chaque exercice, et un dossier output_correction contient les outputs (.png, .shp, etc.) attendus pour chaque exercice. 
Un script 7_Cartographie.R est à la fois le contenu du module 7 (cartographie thématique) et sert de base pour réaliser vos propres tests pour la réalisation de cartes en R. La première partie traite des échelles de couleurs (palettes) en R/ggplot2 et peut être utile en dehors du strict traitement/analyse de données spatiales. 
Données brutes (raw_data)
Les données utilisées dans les slides à titre d’exemple sont aussi celles sur lesquelles se basent les exercices. Ces données sont libres et peuvent être rediffusées, pourvu que la source soient indiquées.
•	Jeu de données Yvel :données spatio temporelles de de qualité de l’eau, délimitation de petits bassins versants, hydrographie, RPG 2018 
•	BD Carto, région 53-Bretagne (IGN)
•	Jeu de données sur les méthaniseurs en France (2020)
•	MNT 25 m des départements bretons (IGN)
•	Jeu de données Naizin : délimitation, extrait image Landsat 8 
 « Cheat-sheets »
Ressources externes, 4 feuilles d’aides pour les packages ggplot, dplyr, tidyr et sf qui sont utilisés au long de cette formation (source : https://www.rstudio.com/resources/cheatsheets/ et https://github.com/rstudio/cheatsheets/blob/master/sf.pdf).  Il est recommandé de les imprimer. Elles peuvent être très utiles pour réaliser les exercices/vos premiers scripts, et permettent d’avoir un aperçu général des méthodes disponibles dans chaque package. 
