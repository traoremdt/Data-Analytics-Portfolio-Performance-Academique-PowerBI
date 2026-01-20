## 🎓 Pilotage de la Performance Académique

### 🎯 Objectif
]Ce projet Power BI analyse les données de 90 étudiants pour convertir des données brutes en indicateurs de décision stratégique.

### 📊 Indicateurs Clés (KPI)
* **Moyenne Générale :** 12,17 / 20.
* **Taux de Réussite :** 69%.
* **Taux d'Échec :** 31%.
* **Équité Sociale :** Écart de seulement 0,13 entre boursiers (4,83) et non-boursiers (4,96).

### 🧠 Analyse Technique (DAX)
Voici les formules principales utilisées pour l'automatisation :
* **Taux de Réussite :** `DIVIDE(CALCULATE(COUNT(F_resultats[Note]), F_resultats[Note] >= 10), COUNT(F_resultats[Note]))` 
* **Moyenne :** `AVERAGE(F_resultats[Note])` 
* **Effectif Unique :** `DISTINCTCOUNT(F_resultats[ID_Etudiant])` 

### 📈 Insights Majeurs
* **Performance par filière :** La Gestion (12,6) et l'Informatique (12,5) surperforment le Droit (11,2).
* **Saisonnalité :** Progression nette des résultats au Semestre 2 (12,60) par rapport au Semestre 1 (11,64).
* **Matières clés :** Le Droit Constitutionnel et la Finance sont les cours les plus suivis (39 étudiants chacun).

### 🛠️ Stack Technique
* **Outils :** Power BI, Power Query.
* **Modélisation :** Schéma en étoile avec table de faits (`F_resultats`) et dimensions (`D_temps`, `D_prof`, `D_etudiant`).
