# I - Introduction

Litoditis marina est un nématode méiobenthique, largement distribué dans les environnements estuariens caractérisés par un fort hydrodynamisme. Commun à travers le monde, cet organisme bactériophage se distingue par une grande variabilité dans ses comportements reproducteurs et sa tolérance aux stress physiologiques. Des études ont également révélé la co-occurrence d'espèces cryptiques au sein de L. marina, suggérant des interactions complexes régies par le principe d’exclusion de Gause. Ces interactions peuvent toutefois évoluer vers une coexistence si un partitionnement efficace des niches écologiques s’établit. Les changements environnementaux, quant à eux, jouent un rôle clé dans la dynamique des communautés, favorisant parfois les compétiteurs moins dominants et modifiant les capacités compétitives des espèces en présence. Enfin, le rôle du microbiome associé à ces organismes dans leur réponse aux perturbations environnementales reste une question cruciale et encore peu explorée.

Afin d'obtenir des informations à ce sujet, une étude à été menée afin d'evaluer l'effet des changements de temperature sur la composition du microbiome.

La méthodologie employée est la suivante : pour chaque température d'exposition, l'ADN du complexe nématodes + microbes a été extrait, puis la région V4 de la petite sous-unité de l'ARNr 16S (une région variable permettant de différencier les espèces) a été amplifiée par PCR. Les séquences des complexes correspondant aux différentes températures ont ensuite été obtenues grâce à un séquençage des amplicons réalisé via la technologie Illumina (Illumina MiSeq, 2 x 300 pb). Les données utilisées pour l'analyse proviennent de ce séquençage Illumina et se présentent sous la forme d'une table d'ASV.

L'objectif de ce projet est de comparer différentes bases de données taxonomiques afin de fournir une évaluation objective sur le choix le plus adapté pour analyser les résultats obtenus dans cette étude.

Trois bases de référence seront examinées : Greengenes, SILVA et RDP.

SILVA contient des informations taxonomiques sur les bactéries, les eucaryotes et les archées. Elle repose principalement sur la phylogénie des petites sous-unités de rRNAs (16S pour les procaryotes et 18S pour les eucaryotes) et permet une classification détaillée jusqu'au niveau de l'espèce.

Greengenes est dédiée aux bactéries et aux archées, avec une classification basée sur la construction automatique d'arbres phylogénétiques de novo, en s'appuyant sur des références existantes (principalement NCBI). Ces arbres sont générés à partir de séquences 16S rRNA issues de bases publiques après vérification de leur qualité.

RDP (Ribosomal Database Project) regroupe des séquences 16S rRNA de bactéries, d'archées et de champignons. Contrairement à SILVA, cette base propose une classification taxonomique qui s’arrête au niveau du genre.

Cette étude permettra d’évaluer les performances de ces trois bases et d’identifier celle qui est la plus pertinente pour le traitement des résultats de cette recherche.


Pour ce faire, différentes analyses seront réalisées sur les données en utilisant les trois bases de données. Ces analyses s'appuieront sur les données collectées pour l'espèce PM4 avec nourriture, comprenant 9 réplicats par température.

# II  - Analyses 

1) Nombre d'assignation selon les bases de données

Calcul du nombre d'assignation ayant été effectué pour chaque base de donnée selon plusieurs critères : 

- Le nombre d'assignation toal 
- Le nombre d'assignation ayant été fait à minima jusqu'au genre 
- Le nombre d'assignation ayant été fait jusqu'à l'espèce 

Resultat sous forme de tableau 

2) Assignation de l'espece la plus abondante et du genre le plus abondant

Verification de l'identité de l'espèce correspondant à l'ASV la plus frequente pour chaque température en fonction des 3 bases de reference.

METTRE TABLEAU RESULTAT 

On observe que l'espece la plus abondante est la meme pour toutes les températures. En revanche, elle est differente selon la base de données, GG2 nous donne rumoiensis alors que SILVA nous donne casei et RDP n'assigne aucun espece à l'ASV la plus fréquente.
Pour les genre, on obtient les meme genre pour toutes les base de données et toutes les températures.


3) Diagramme de Venn 

pb suffixes

4) Richesse specifique + permanova 

Création de graphiques permettant d'observer la richesse specifique à chaque temperature et pour chaque base de données. 

METTRE LES GRAPH 

Les graphiques montrent que, pour une même température, la diversité des espèces et des genres reste presque identique quelle que soit la base de données utilisée.
En revanche, une variation selon les températures est visible : les trois bases de données indiquent une abondance plus élevée à 20 °C.

Verification statistique des resultats à l'aide d'un test Kruskal Wallis.



# Conclusion

Le compromis entre la qualité et la quantité des assignations fait de Greengenes 2 (GG2) le meilleur choix. Cette base offre un nombre d’assignations jusqu’au niveau de l’espèce relativement élevé et performant, tout en permettant d’attribuer une espèce à l’ASV la plus abondante. En comparaison, RDP présente le plus grand nombre d’assignations jusqu'à l’espèce, mais ne parvient pas à identifier une espèce pour l’ASV la plus dominante. Quant à SILVA, bien qu’elle affiche le plus faible nombre d’assignations jusqu’à l’espèce, elle a l’avantage d’attribuer une espèce à l’ASV la plus fréquente.

- parler des suffixes base GG2

# FAIRNESS ?

