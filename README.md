# **Housing Project**

Ce projet est réalisé dans le cadre de la formation **365 Data Science** et constitue une partie de l'examen du cours *Introduction à la programmation R*. Grâce à ce projet, j'ai obtenu mon certificat pour ce cours. Le but est d'effectuer une analyse statistique et visuelle des données immobilières tout en appliquant des concepts fondamentaux de la programmation en R.

---

## **Objectifs du projet**
1. Explorer les données immobilières et calculer des statistiques descriptives.
2. Visualiser les données à l'aide de graphiques.
3. Effectuer des tests d'hypothèses pour comparer des groupes.
4. Construire un modèle de régression linéaire pour prédire la valeur médiane des maisons.

---

## **Structure du projet**
### **Partie 1 : Analyse des données**
1. Chargement des bibliothèques nécessaires :
   - `ggplot2`
   - `dplyr`
   - `car`
2. Importation et exploration des données. Cela inclut la gestion des valeurs manquantes, aberrantes, doublons, etc. Les données proviennent de la source **housing_data**, fournies par **365 Data Science**.
3. Calcul des statistiques descriptives :
   - Moyenne, médiane, mode et écart-type.
   - Calcul des corrélations entre paires de variables.

### **Partie 2 : Visualisation des données**
Création d'un histogramme stylisé des prix des maisons avec 8 classes pour représenter la distribution.

### **Partie 3 : Test d'hypothèse**
1. Comparaison des groupes de taux de criminalité définis comme "élevés" et "bas" en fonction de la médiane.
2. Vérification des hypothèses pour un test t (normalité et homogénéité de la variance).
3. Exécution d'un test t indépendant.

### **Partie 4 : Régression linéaire**
Modélisation pour prédire la valeur médiane des maisons en fonction de la variable "moyenne de chambres".

---

## **Données**
Les données utilisées pour ce projet, appelées **housing_data**, sont disponibles dans ce dépôt. Vous pouvez les télécharger [ici](housing_data.csv) pour les utiliser dans votre analyse.

Veuillez noter que ces données ne sont pas incluses dans ce dépôt pour des raisons de confidentialité.

---

## **Examen et Certification**

Ce projet inclut un examen de 12 questions qui a été réalisé dans le cadre de la formation. Les réponses à ces questions sont les suivantes :

1. **Question 1 :** Vous êtes un grand fan du langage de programmation R et de la bibliothèque ggplot2 en particulier, et vous connaissez tous les faits et anecdotes qui y sont liés. Laquelle des affirmations suivantes (le cas échéant) sur ggplot2 n'est PAS vraie ?  
   **Réponse :** Toutes les affirmations sont correctes.

2. **Question 2 :** Pour analyser les données que vous avez reçues, vous décidez d'examiner la relation entre deux variables - prix et surface. Pour ce faire, vous décidez de créer un nuage de points basé sur les données, avec la Surface sur l'axe des x et le Prix sur l'axe des y. Remplissez les mots manquants dans le code pour créer un nuage de points :  
   **Réponse :** `df_real_estate; area...ft..; price;`

3. **Question 3 :** Observez la version suivante du nuage de points. Une troisième variable a été incorporée dans le graphique par la couleur. Quelle est la troisième variable ?  
   **Réponse :** Propriété de bâtiment.

4. **Question 4 :** Observez la version suivante du nuage de points. Quelle fonction combinée avec l'objet de nuage de points original peut produire cette image ?  
   **Réponse :** `stat_smooth()`

5. **Question 5 :** En analysant les données, que diriez-vous sur la corrélation et la covariance des deux variables, Surface et Prix ?  
   **Réponse :** Les variables sont corrélées et il y a une covariance positive.

6. **Question 6 :** Quel est le coefficient de corrélation du Prix et de la Surface, arrondi à deux décimales ?  
   **Réponse :** 0.95.

7. **Question 7 :** Complétez la définition suivante du package dplyr : Partie du tidyverse, spécialisée dans les outils de manipulation de données, comme...  
   **Réponse :** Tout ce qui précède (Explication : Le package dplyr peut être utilisé pour filtrer, muter, ainsi que résumer les données.)

8. **Question 8 :** Laquelle des séquences suivantes constitue une séquence valide de couches ggplot ?  
   **Réponse :** données, esthétiques, géométrie, coordonnées. (Explication : Il y a sept couches au total dans ggplot. Les trois premières - données, esthétiques et géométrie - sont obligatoires et doivent apparaître dans cet ordre. Les quatre restantes - facettes, statistiques, coordonnées et thème - sont facultatives et ici l'ordre n'est pas strict.)

9. **Question 9 :** Vous souhaitez explorer les données plus avant, donc vous envisagez de créer un histogramme sur la variable que vous pensez être la plus révélatrice des données. Quand un histogramme est-il le choix le plus approprié pour la visualisation des données ?  
   **Réponse :** Lorsque vous êtes intéressé par les fréquences.

10. **Question 10 :** Examinez l'image de l'histogramme. En regardant les données, laquelle des descriptions suivantes de l'histogramme est la plus appropriée ?  
    **Réponse :** Un histogramme du Prix avec une largeur de classe de 50.

11. **Question 11 :** Laquelle des affirmations suivantes est la plus susceptible d'être vraie, basée sur l'histogramme du Prix ?  
    **Réponse :** L'histogramme a une asymétrie à droite, ce qui signifie que la médiane est inférieure à la moyenne.

12. **Question 12 :** Quelle est la moyenne, la médiane et le mode de la variable Prix ?  
    **Réponse :** MOYENNE = 249.08, MÉDIANE = 281.17, MODE = 460.00.

### Certification obtenue
J'ai obtenu ma certification pour le cours *Introduction à la programmation R* grâce à la réussite de cet examen.

### Vidéo explicative
Pour une explication détaillée de ce projet et des concepts abordés, vous pouvez consulter la vidéo explicative [ici](My_housingProject_video).

## **Pré-requis**
### **Outils**
- R (version 4.2 ou plus récente). Pour ma part, j'ai travaillé avec R lié à Jupyter Notebook, mais vous pouvez utiliser RStudio.
- Un IDE tel que RStudio.

### **Packages à installer**
Exécutez les commandes suivantes si vous n'avez pas encore installé les bibliothèques requises :
```R
install.packages(c("ggplot2", "dplyr", "car"))