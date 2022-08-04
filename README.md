Ces scripts sont destinés à l'analyse statistique de séquences préalablement traitée sous forme d'ASV.

Le traitement des séquences à l'aide du package DADA2 permet l'obtention d'une matrice d'abondance d'ASV et d'une table de taxonomie.

**Raréfaction.Rmd:** Le choix des analyses a réalisé par la suite peut nécessiter de raréfier la matrice d'abondance. Ce script permet de réaliser des courbes de raréfactions afin de déterminer la valeur de raréfaction appropriée afin de ne pas perdre une trop grande par de la diversité. Raréfier ce n’est pas automatique, assurer vous de la nécessitée de cette étape.

**diversité phylo.Rmd:** Le script DADA2 fourni dans le répertoire "traitement RAW" permet le calcul de l'arbre phylogénétique associé aux ASV de votre communauté. Vous pouvez déduire de cet arbre des matrices de distance phylogénétique permettant d'analyser la différence phylogénétique entre les communautés de vos différents échantillons. Ce script explique les différentes méthodes possibles et leurs réalisations.

**Transformation chimie.Rmd:** Script permettant de transformer les données environnementales associées a vos échantillons afin de leur donner une distribution proche de la normale, ceci est nécessaire est nécessaire pour les analyses paramétriques. La transformation utilisée est celle de BOX COX. La colinéarité des variables est ensuite testée puis une PCA permet de résumer les variables colinéaires par les valeurs de l'axe de PCA qui leur est associé.

**dbRDA.Rmd:** Script permettant la réalisation d'une dbRDA, analyse multivariée permettant de déterminer la part de variance dans une communauté associée a des variables environnementales connues. Celle si nécessite un nombre d'échantillons plus grand que le nombre de variables environnementales testées.

**Coocurences.Rmd:** script permettant de tester la corrélation dans l'abondance relative de 2 communautés dans les mêmes échantillons afin de déterminer de potentiel interactions.

