# Analyse de la Qualité de l'Air - Big Data & Deep Learning

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.10%2B-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

## 📋 Description

Ce projet d'analyse de données se concentre sur l'étude de la qualité de l'air en utilisant des techniques de Big Data et de Deep Learning. L'objectif principal est de développer un modèle prédictif performant capable d'analyser et de prédire les niveaux de pollution atmosphérique basé sur plus de 12 variables environnementales.

## 🎯 Objectifs

- **Analyse exploratoire** : Comprendre la structure et les patterns des données de qualité de l'air
- **Corrélation des variables** : Identifier les relations entre les différents polluants et facteurs météorologiques
- **Modélisation prédictive** : Développer et comparer plusieurs modèles de machine learning et deep learning
- **Évaluation comparative** : Analyser les performances des différents algorithmes

## 📊 Dataset

Le projet utilise le dataset **AirQualityUCI** qui contient :
- **Source** : Données de qualité de l'air UCI
- **Variables** : Plus de 12 variables environnementales et météorologiques
- **Format** : CSV avec séparateur `;` et décimales `,`
- **Période** : Données temporelles avec horodatage

### Variables principales :
- **Polluants primaires** : CO(GT), NOx(GT), NO2(GT)
- **Polluants secondaires** : Benzène, hydrocarbures
- **Facteurs météorologiques** : Température, humidité relative
- **Variables temporelles** : Date et heure

## 🗂️ Structure du Projet

```
air_quality/
├── .github/
│   ├── workflows/
│   │   └── ci.yml                 # GitHub Actions CI/CD
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md          # Template pour rapporter des bugs
│       └── feature_request.md     # Template pour demander des fonctionnalités
├── data/
│   ├── AirQualityUCI.csv          # Dataset principal
│   └── AirQualityUCI.xlsx         # Dataset format Excel
├── air_quality.ipynb              # Notebook principal d'analyse
├── air_quality_updated.ipynb      # Version mise à jour avec améliorations
├── .gitignore                     # Fichiers à ignorer par Git
├── requirements.txt               # Dépendances Python
├── LICENSE                        # Licence MIT
├── CONTRIBUTING.md                # Guide de contribution
└── README.md                      # Documentation du projet
```

## 🔧 Technologies Utilisées

### Libraries Python
- **Data Science** : `pandas`, `numpy`
- **Visualisation** : `matplotlib`, `seaborn`
- **Machine Learning** : `scikit-learn`
- **Deep Learning** : `tensorflow`, `keras`
- **Preprocessing** : `MinMaxScaler`, `StandardScaler`

### Modèles Implémentés
#### Machine Learning Traditionnel
- **Linear Regression** : Modèle de base linéaire
- **Random Forest Regressor** : Modèle d'ensemble
- **Support Vector Regression (SVR)** : Modèle à vecteurs de support
- **MLP Regressor** : Réseau de neurones simple

#### Deep Learning
- **Simple RNN** : Réseau récurrent de base
- **LSTM** : Long Short-Term Memory
- **GRU** : Gated Recurrent Unit
- **BiLSTM** : LSTM bidirectionnel

## 🚀 Installation et Utilisation

### Prérequis
```bash
python >= 3.8
jupyter notebook
```

### Installation des dépendances
```bash
pip install -r requirements.txt
```

### Lancement du projet
1. Cloner le repository
```bash
git clone <votre-repository-url>
cd air_quality
```
2. Installer les dépendances
```bash
pip install -r requirements.txt
```
3. Ouvrir le notebook principal : `air_quality.ipynb`
4. Exécuter les cellules séquentiellement

## 📈 Méthodologie

### 1. **Exploration des Données**
- Analyse de la structure du dataset
- Identification et traitement des valeurs manquantes
- Statistiques descriptives

### 2. **Préprocessing**
- Nettoyage des données
- Normalisation avec MinMaxScaler et StandardScaler
- Création de séquences temporelles pour les modèles RNN

### 3. **Analyse des Corrélations**
- Matrice de corrélation
- Analyse des relations entre polluants
- Identification des variables les plus prédictives

### 4. **Modélisation**
- Division train/test
- Entraînement de multiples modèles
- Validation croisée
- Optimisation des hyperparamètres

### 5. **Évaluation**
- Métriques de performance : MSE, MAE, R²
- Comparaison des modèles
- Visualisation des prédictions

## 📊 Résultats

Les notebooks incluent :
- **Visualisations** : Graphiques de corrélation, distributions, séries temporelles
- **Métriques de performance** : Comparaison détaillée des modèles
- **Prédictions** : Visualisation des résultats sur données de test

## 🎓 Contexte Académique

Ce projet s'inscrit dans le cadre d'un cours de **Big Data & Deep Learning** et traite les aspects suivants :
1. **Dataset complexe** : Gestion de plus de 12 variables
2. **Contexte et corrélations** : Analyse approfondie des relations
3. **Problématique Deep Learning** : Choix et justification des algorithmes
4. **Application pratique** : Mise en œuvre sur données réelles
5. **Conclusions** : Synthèse et recommandations

## 🔍 Points d'Amélioration

- **Feature Engineering** : Création de nouvelles variables dérivées
- **Hyperparameter Tuning** : Optimisation plus poussée des modèles
- **Ensemble Methods** : Combinaison de plusieurs modèles
- **Real-time Prediction** : Développement d'une API de prédiction

## 📝 Notes

- Les données contiennent des valeurs manquantes codées `-200`
- Le préprocessing inclut une interpolation pour combler les lacunes
- Les modèles deep learning utilisent des séquences temporelles
- La validation se fait par validation croisée k-fold

## 👨‍💻 Auteur

Projet réalisé dans le cadre d'un cours académique de Big Data & Deep Learning.

## 🤝 Contribution

Les contributions sont les bienvenues ! Consultez le fichier [CONTRIBUTING.md](CONTRIBUTING.md) pour plus de détails.

### Comment contribuer :
1. Fork le projet
2. Créez une branche pour votre feature (`git checkout -b feature/AmazingFeature`)
3. Commitez vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrez une Pull Request

## 📄 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

*Pour toute question ou amélioration, n'hésitez pas à ouvrir une issue ou proposer une pull request.*
