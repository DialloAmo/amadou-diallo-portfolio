# Profile & Projets — Diallo Amadou

Bienvenue dans mon portfolio junior Data Scientist / ML Engineer / Research Engineer.  
Vous trouverez ici une sélection de projets réalisés de bout en bout : **analyse**, **préprocessing**, **modélisation**, **évaluation**, et selon les cas **optimisation**, **industrialisation** et **Topology Data Analysis (TDA)**.

## Highlights
- **Projets ML de bout en bout** : EDA → preprocessing → modèles → évaluation → optimisation (pipelines scikit-learn).
- **Approche orientée impact** : choix de métriques adaptées (ex. **Recall** en santé / classification), analyse des erreurs (confusion matrix) et recommandations.
- **Structuration** : repos reproductibles (conda/env), code organisé (`src/`), documentation claire (README + notebooks).
- **Santé & données sensibles** : en parallèle, stage (Avril → septembre) en laboratoire sur **Cartographie dynamique de la leucémie lymphoïde chronique : des indicateurs biologiques aux paramètres cliniques et inversement par l'approche TDA et Machine Learning**, un stage où l’on applique le machine learning et des méthodes d’ingénierie de recherche à des problèmes de biologie computationnelle.

**Ce que vous pouvez regarder en priorité :**
- Les **README** de chaque projet (objectif + résultats + limites)
- Les notebooks dans `notebooks/` (EDA + modèles)
- La structure de code dans `src/` (pipeline, fonctions, reproductibilité)

---

## STAGE
### Sujet: Cartographie dynamique de la leucémie lymphoïde chronique : des indicateurs biologiques aux paramètres cliniques et inversement par l’approche TDA et Machine Learning

### 1) Contexte: 
La leucémie lymphoïde chronique (LLC) est une maladie hétérogène caractérisée par une évolution clinique variable, difficile à prédire à partir des données biologiques statiques. La complexité et la haute dimensionnalité des données multi -échelles (génomique, transcriptomique, clinique) ainsi que la nature dynamique de la maladie appellent à des approches mathématiques avancées capables de capturer des structures géométriques et topologiques sous-jacentes, souvent masquées par les méthodes classiques.

### 2) Objectif du stage: 
L’objectif de ce stage en mathématiques appliquées est de développer **un pipeline d’analyse intégrative** combinant **Topological Data Analysis (TDA) et Machine Learning (ML)** pour établir une cartographie bidirectionnelle et dynamique entre les marqueurs biologiques et les paramètres cliniques dans la LLC. Le travail visera à :    
- **De la biologie vers le clinique (prédiction) :** Utiliser la TDA (notamment l’homologie persistante et les représentations de graphes de voisinage) pour extraire des invariants topologiques des espaces de données biologiques (mutations, expressions géniques). Ces caractéristiques topologiques serviront de features robustes et stables pour entraîner des modèles de ML (forêts aléatoires, réseaux de neurones, modèles à noyaux) afin de prédire l’évolution clinique, la réponse thérapeutique ou le risque de progression.  
- **Du clinique vers la biologie (inférence et interprétation) :** À partir des trajectoires cliniques, reconstruire les espaces de paramètres biologiques latents à l’aide de méthodes d’apprentissage non supervisé (cartographie par UMAP/t-SNE enrichis par des descripteurs topologiques ). Mettre en œuvre des modèles inversibles (invertible neural networks) ou des techniques de rétro-propagation/génération conditionnelle (GANs conditionnels, VAEs) pour proposer des configurations biologiques plausibles associées à un profil clinique observé.

### 3) Méthodologie envisagée :
- **Pré-traitement et intégration** des données multi-omiques et cliniques (cohortes publiques ou collaboratives).  
- **Extraction de features topologiques :** construction de complexes simpliciaux à partir des points de données (nuages de points biologiques), calcul des diagrammes de persistance et transformation en vecteurs (persistence images, persistence landscapes) ou graphes.   
- **Apprentissage automatique hybride TDA+ML :** entraînement de modèles prédictifs sur les représentations topologiques, validation croisée, interprétation des caractéristiques importantes.  
- **Modélisation dynamique :** combinaison de modèles à base d’équations différentielles (dynamiques des populations cellulaires) et de techniques de ML pour calibrer les paramètres à partir de données temporelles. La TDA pourra être utilisée pour caractériser l’évolution de la forme des attracteurs du système au cours du temps.  
- **Validation biologique :** interprétation des résultats en collaboration avec des biologistes/cliniciens, recherche de corrélats biologiques aux structures topologiques identifiées.  

### 4) Compétences mobilisées :
- Mathématiques : Topologie algébrique (bases de TDA), analyse de données, systèmes dynamiques.
- Informatique : Programmation Python avancée (bibliothèques : GUDHI, Ripser, Scikit-learn, TensorFlow/PyTorch, DyNeR, etc.).
- Machine Learning et analyse statistique.
- Travail interdisciplinaire en modélisation biomédicale.

## Projets

### 1) COVID Analysis — Diagnostic Prediction (Classification)
**But :** prédire la positivité au SARS-Cov-2 à partir de variables cliniques/biologiques.  
**ML :** classification binaire, pipelines scikit-learn, optimisation hyperparamètres, focus sur **Recall** (réduction des faux négatifs).  
Repo : https://github.com/DialloAmo/covid_analysis

### 2) Customer Churn Prediction & Business Insights
**But :** prédire le churn et produire des **insights** actionnables pour la rétention client.  
**ML :** modèles de classification + analyse des facteurs (feature importance / interprétabilité) + recommandations business.  
Repo : https://github.com/DialloAmo/Customer_Churn_Prediction

### 3) Credit Risk Scoring — Statistical & ML Models
**But :** estimer le risque de défaut et construire un scoring robuste et explicable.  
**ML :** modèles statistiques + ML, gestion du déséquilibre, calibration/thresholding, interprétabilité.  
Repo : https://github.com/DialloAmo/Credit_Risk_Scoring

### 4) End-to-End ML Pipeline — Prediction + Monitoring
**But :** mettre en place une approche “production-like” : entraînement → prédiction → monitoring.  
**ML Ops :** pipeline reproductible, suivi des performances, détection de dérive, alerting (selon avancement).  
Repo : https://github.com/DialloAmo/End_to_End_ML_Pipeline

---

## Compétences mises en œuvre

**Data & Analyse**
- Data cleaning, EDA, visualisation, data quality
- Feature engineering, gestion des valeurs manquantes

**Machine Learning**
- Classification (scikit-learn), pipelines, cross-validation
- Déséquilibre de classes, hyperparameter tuning (Grid/RandomizedSearch)
- Évaluation : Precision / Recall / F1, confusion matrix, PR/ROC curves

**Reproductibilité / Projet**
- Structuration de repo (`data/`, `notebooks/`, `src/`)
- Environnement conda (`environment.yml`)
- README clair + méthodo documentée

---

## Roadmap (2026)
- ⏳ Stage : topology-aware-ml-for-cll
topology-aware-ml-for-cll/
├── README.md
├── .gitignore
├── requirements.txt
├── notebooks/
│   ├── 00_setup.ipynb
│   ├── 01_data_audit.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_tda_features.ipynb
│   ├── 04_bio_to_clinical_prediction.ipynb
│   ├── 05_clinical_to_bio_inference.ipynb
│   └── 06_dynamic_modeling.ipynb
├── src/
│   ├── data/
│   ├── topology/
│   ├── models/
│   ├── evaluation/
│   └── visualization/
├── data/
│   ├── raw/
│   ├── interim/
│   └── processed/
├── figures/
├── reports/
└── references/ 
- ✅ Projet 1 : COVID Analysis — classification + tuning
- ✅ Projet 2 : Customer Churn Prediction & Business Insights
- ⏳ Projet 3 : Credit Risk Scoring (stat + ML + calibration + interprétabilité)
- ⏳ Projet 4 : End-to-End ML Pipeline (prediction + monitoring)

---

## Objectif & Disponibilités
Je cherche un **CDD** en **junior Data Scientist / ML Engineer / Research Engineer**, idéalement en complément de mon stage en laboratoire en temps patiel (**Avril → septembre**).  
Objectif : **Evoluer vers un CDI** à l’issue du stage (fin septembre).

## Ouvert aux missions : 
Modélisation & decision, data pipeline, Analyse de données, Reporting Avancé, Machine Learning Appliqué, Recheche & Développement Data 

## Contact :
- GitHub : https://github.com/DialloAmo  
- LinkedIn : (ajoute ton lien)
- Email : amadoudiallodjikesse@gmail.com

