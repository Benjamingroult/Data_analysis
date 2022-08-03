Ces scripts sont déstiné a l'annalyse statistique de séquences préalablement traité sous forme d'ASV.

Le traitement des séquences à l'aide du package DADA2 permet l'obtention d'une matrice d'abondance d'ASV et d'une table de taxonomie.

**Raréfaction.Rmd:** Le choix des annalyses a réaliser par la suite peut necessiter de raréfier la matrice d'abondance. Ce script permet de réaliser des courbes de raréfactions afin de déterminer la valeur de raréfaction approprié afin de ne pas perdre une trop grande par de la diversité. Raréfier c'est pas automatique, assurer vous de la necessitée de cette étape.

**diversité phylo.Rmd:** Le script DADA2 fourni dans le répertoire "traitement RAW" permet le calcul de l'arbre phylogénétique associé aux ASV de votre communautés. Vous pouvez déduire de cet arbre des matrices de distance phylogénétique permettant d'annalyser la différence phylopgénétique entre les communautés de vos différents échantillons. Ce script explique les différentes méthodes possible et leurs réalisation.

**Transformation chimie.Rmd:** Script permettant de transformer les donnée environnementales associées a vos échantillons afin de leurs donner une distribution proche de la normale, ceci est necessaire est necessaire pour les annalyses paramétrique. La transformation utilisée est celle de BOX COX. La colinéaritée des variables est ensuite testée puis une PCA permet de résumer les variables colinéaire par les valeurs de l'axe de PCA qui leurs est associés.

**dbRDA.Rmd:** Script permettant la réalisation d'une dbRDA, annalyses multivariée permettant de déterminer la part de variance dans une commuanutés associées a des variables environnementales connues. Celle si necessite un nombre d'échantillons plus grand que le nombre de variables environnementales testée.

**Coocurences.Rmd:** script permettant de tester la corrélation dans l'abondance relatives de 2 communautés dans les mêmes échantillons afin de déterminer de pottentiels interactions.

