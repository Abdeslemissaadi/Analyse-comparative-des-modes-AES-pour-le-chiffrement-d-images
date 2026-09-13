# Analyse-comparative-des-modes-AES-pour-le-chiffrement-d-images

Ce projet consiste en un travail pratique de cryptographie visant à évaluer et comparer les performances des 5 modes d'opération du chiffrement symétrique AES-128 (ECB, CBC, CFB, OFB et CTR) appliqués à une image numérique (Paris8.jpg).

L'expérimentation s'articule autour de quatre axes principaux :

Chiffrement de l'image : Chargement du fichier original et application successive des 5 modes de chiffrement d'AES.

Analyse de l'entropie : Évaluation de la répartition statistique des données chiffrées pour mesurer leur niveau d'aléatoire et vérifier l'absence de motifs résiduels.

Analyse de la propagation d'erreurs : Altération volontaire d'un octet dans le fichier chiffré pour observer l'impact sur le déchiffrement (avec et sans compression préalable), illustrant ainsi le comportement de chaque mode face au bruit ou à la corruption de données.

Synthèse et visualisations : Génération de graphiques comparatifs pour conclure sur le mode d'opération le plus adapté au chiffrement de données visuelles.

Objectifs pédagogiques :

Mettre en évidence les vulnérabilités du mode ECB, qui conserve la structure visuelle de l'image en chiffrant les blocs identiques de manière déterministe.

Démontrer l'efficacité des modes CBC, CFB, OFB et CTR pour produire un bruit parfaitement uniforme.

Illustrer concrètement les concepts fondamentaux de la cryptographie moderne : la confusion et la diffusion selon Claude Shannon, ainsi que le principe de Kerckhoffs.

Environnement technique :

Langage et plateforme : Python (Google Colab)

Bibliothèque cryptographique : pycryptodome (implémentation de l'AES)

Traitement d'images et visualisations : Pillow et matplotlib
