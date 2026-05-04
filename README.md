# 🚀 Analyse Multi-Modale du Transport : Rapport de Performance & Insights Stratégiques

### **Test Technique - Candidature Alternance Data**
**Auteur :** Israa Mokadem

---

## 🧐 Présentation du Projet
Ce mini-projet a été réalisé dans le cadre du processus de recrutement de **Tictactrip**. L'objectif est d'analyser les dynamiques de prix et de durée des trajets à travers trois modes de transport : **Train, Bus et Covoiturage**.

### **La Problématique**
> *"Comment le rapport entre le coût du trajet et la rapidité évolue-t-il selon la distance, et dans quelle mesure les facteurs externes comme la saisonnalité influencent-ils cette efficacité ?"*

---

## 🛠️ Ce qui rend ce projet unique
Au-delà de la simple manipulation de données, ce notebook intègre une approche **Data Engineering** et **Business Intelligence** complète :

* **🔍 Audit de Qualité (Data Quality) :** Avant toute analyse, un rapport d'audit identifie les anomalies (valeurs manquantes, incohérences temporelles, doublons) pour garantir la fiabilité des résultats.
* **📏 Ingénierie de la Distance (Formule de Haversine) :** La distance n'étant pas fournie, j'ai implémenté le calcul "à vol d'oiseau" entre les villes à partir de leurs coordonnées GPS (latitude/longitude).
* **📅 Enrichissement par API Externe :** Intégration des jours fériés pour mesurer l'impact de la saisonnalité sur la fluctuation des tarifs, ajoutant une dimension contextuelle indispensable à l'analyse.
* **📊 Segmentation Stratégique :** Regroupement des trajets par tranches de distance (0-200km, 201-800km, etc.) pour identifier les leaders de marché sur chaque segment.

---

## 📈 Insights Clés (Extrait de l'étude)
* **Courte distance (0-200 km) :** Le covoiturage domine largement avec le meilleur rapport prix/temps.
* **Moyenne distance (201-800 km) :** Zone de forte concurrence où le Train commence à justifier son surcoût par un gain de temps massif.
* **Arbitrage Utilisateur :** Mise en évidence d'une forte dispersion des tarifs ferroviaires, révélant une stratégie de *Yield Management* plus agressive que pour le bus ou le covoiturage.

---

## ⚙️ Installation et Utilisation

### **Prérequis**
* Python 3.x
* Librairies : `pandas`, `numpy`, `matplotlib`, `seaborn`, `geopy` (ou `math`).

### **Exécution**
1.  Placez les 4 fichiers CSV fournis (`ticket_data.csv`, `cities.csv`, `providers.csv`, `stations.csv`) dans le répertoire du notebook.
2.  Lancez le notebook `tictac_trip_.ipynb`.
3.  Exécutez toutes les cellules pour générer l'audit et les visualisations interactives.

---

## 🤝 Contact
**Israa Mokadem** – Futur Étudiante en Data et cyber Paris 8 
contact: isramokaddem0@gmail.com |    0635074677
*Projet réalisé avec rigueur et passion pour l'optimisation de la mobilité.*

---

> **Note pour l'examinateur :** Le code a été structuré pour être modulaire et facilement industrialisable. Chaque étape de transformation de données (conversion monétaire, formatage temporel, jointures) est documentée pour assurer la maintenabilité de la pipeline.
