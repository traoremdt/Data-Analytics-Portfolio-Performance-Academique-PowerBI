## 🎓 Pilotage de la Performance Académique

### 🎯 Objectif
[cite_start]Ce projet Power BI analyse les données de 90 étudiants pour convertir des données brutes en indicateurs de décision stratégique[cite: 7, 20].

### 📊 Indicateurs Clés (KPI)
* [cite_start]**Moyenne Générale :** 12,17 / 20[cite: 38].
* [cite_start]**Taux de Réussite :** 69%[cite: 41].
* [cite_start]**Taux d'Échec :** 31%[cite: 42].
* [cite_start]**Équité Sociale :** Écart de seulement 0,13 entre boursiers (4,83) et non-boursiers (4,96)[cite: 91, 92].

### 🧠 Analyse Technique (DAX)
Voici les formules principales utilisées pour l'automatisation :
* [cite_start]**Taux de Réussite :** `DIVIDE(CALCULATE(COUNT(F_resultats[Note]), F_resultats[Note] >= 10), COUNT(F_resultats[Note]))` [cite: 40]
* [cite_start]**Moyenne :** `AVERAGE(F_resultats[Note])` [cite: 38]
* [cite_start]**Effectif Unique :** `DISTINCTCOUNT(F_resultats[ID_Etudiant])` [cite: 36]

### 📈 Insights Majeurs
* [cite_start]**Performance par filière :** La Gestion (12,6) et l'Informatique (12,5) surperforment le Droit (11,2)[cite: 48, 50].
* [cite_start]**Saisonnalité :** Progression nette des résultats au Semestre 2 (12,60) par rapport au Semestre 1 (11,64)[cite: 66].
* [cite_start]**Matières clés :** Le Droit Constitutionnel et la Finance sont les cours les plus suivis (39 étudiants chacun)[cite: 89].

### 🛠️ Stack Technique
* [cite_start]**Outils :** Power BI, Power Query[cite: 4, 18].
* [cite_start]**Modélisation :** Schéma en étoile avec table de faits (`F_resultats`) et dimensions (`D_temps`, `D_prof`, `D_etudiant`)[cite: 25, 27, 28].
