# Certification de Francis Pradel : cohorte DSFS-FT-35 chez [JEDHA](https://www.jedha.co/formations/formation-data-scientist)

## Dépôt descriptif pour les projets de données du cursus Fullstack de Jedha (DSFS-FT-35)

### pré requis pour lancer l'évaluation

Il est necessaire d'avoir installer la version Python 3.12 sur sa machine.
Se placer dans un répertoire propre et vide d'évaluation. Sous Linux ou Mac OS, saisir les commandes ci-dessous

```bash
python3.12 -m venv certification
source certification/bin/activate
pip install --upgrade pip
pip install -e git+https://github.com/pradelf/fpcia.git#egg=fpcia


```

à l'issue de ces opérations, vous aurez la libraire python nécessaire pour l'execution des projets : FPCIA [https://github.com/pradelf/fpcia](https://github.com/pradelf/fpcia)

- Kayak : [https://github.com/pradelf/kayak](https://github.com/pradelf/kayak)
- Speed Dating : [https://github.com/pradelf/speeddating](https://github.com/pradelf/speeddating)
- Conversion Challenge : [https://github.com/pradelf/conversion-rate-challenge](https://github.com/pradelf/conversion-rate-challenge)
- Walmart Sales : [https://github.com/pradelf/Walmart-sales](https://github.com/pradelf/Walmart-sales)
- Uber Pickups : [https://github.com/pradelf/uberpickups](https://github.com/pradelf/uberpickups)
- ATT Spam Detector : [https://github.com/pradelf/att](<https://github.com/pradelf/att>)
- Get Around : [https://github.com/pradelf/getaround](https://github.com/pradelf/getaround)]
- OASIS (projet collectif) : [https://github.com/pradelf/oasis](https://github.com/pradelf/oasis)

Le projet [Steam](https://github.com/pradelf/steam) est particulier car il est nécessaire de la faire executer dans l'environnement [Databricks](https://www.databricks.com/fr)
si vous voulez exporter les dépendances des projets, vous pouvez utiliser la commande :

```bash
pip freeze -l git+https://github.com/pradelf/fpcia.git@6d2560ca7e97f6aa67a97c89445da45907015b30#egg=fpcia
```

Vous pouvez vérifer votre environnement local d'évaluation avec la commande ```pip config list -v``` qui vous donne votre configuration local de recherche de Python et des librairies utilisées.

##  💾 Projets de Data Science & Machine Learning

###  🧱 Bloc 1. Construction, alimentation et mise en place d'une infrastructure de gestion de données

#### Kayak

- Extraction automatisée des informations sur les hôtels et la météo pour une liste donnée de villes
- Stockage des données nettoyées dans AWS S3, puis transfert vers une base AWS RDS
- Requêtes SQL pour sélectionner les meilleures villes selon les conditions météo
- Génération de cartes interactives illustrant les températures quotidiennes et les gammes de prix des hôtels.

##### Tech Stack

APIs · Scrapy · Boto3 · AWS S3 · AWS RDS · SQL · SQLAlchemy · Plotly

### 🔍 Bloc 2. Analyse exploratoire, descriptive et inférentielle de données (EDA)

####  Speed Dating

- Exploration d’un jeu de données de speed dating
- Identification des facteurs influençant la probabilité d’obtenir un second rendez-vous.

#####  Tech Stack

Pandas · Numpy · Plotly · Matplotlib

### 🤖 Bloc 3. Analyse prédictive de données structurées par l'intelligence artificielle (IA & Machine Learning)

#### Conversion Challenge

- Modélisation du taux de conversion d’une newsletter à partir de variables déséquilibrées

#### Walmart Sales

- Estimation des ventes hebdomadaires des magasins
- Interprétation des indicateurs économiques pour planifier les campagnes marketing

####  Uber Pickups

- Optimisation du temps d’attente des clients
- Création d’algorithmes de détection de zones chaudes (hot-zones) selon l’heure de la journée

##### Tech Stack

Scikit-learn · XGBoost · Régression linéaire / logistique · Arbres de décision · Forêts aléatoires · Boosting · GridSearch · Validation croisée · K-Means · DBSCAN · Mélange gaussien

### 💬 Bloc 4. Analyse prédictive de données non-structurées par l'intelligence artificielle

#### AT&T Spam Detector

- Développement d’un modèle de deep learning détectant automatiquement les spams selon le contenu textuel
- Traitement complet du langage naturel (NLP) : tokenisation, lemmatisation, encodage, embedding

##### Tech Stack

PyTorch · Transformers · NLP

### 🏭 Bloc 5 : Industrialisation d'un algorithme d'apprentissage automatique et automatisation des processus de décision

### Get Around
- Analyser les retards de restitution des véhicules afin de mesurer leur impact sur la satisfaction client et la planification des locations suivantes.
- Déterminer le délai minimal optimal entre deux locations pour réduire les frictions tout en préservant les revenus des propriétaires et de la plateforme.
- Développer un modèle de prédiction et une API /predict pour optimiser la tarification des locations grâce au Machine Learning.

##### Tech Stack

APIs · Docker · MLFlow · Streamlit · Plotly

### 🏝️ Bloc 6. Direction de projets de gestion de données (Projet collectif)

#### Oasis

- Ce projet vise à prédire les prix de l’immobilier, en se concentrant principalement sur l’impact des événements climatiques.
- Notre objectif est d’identifier les zones sûres et rentables en analysant comment différents phénomènes météorologiques et climatiques influencent la valeur des biens.
- À mesure que le projet évoluera, nous prévoyons d’intégrer d’autres événements majeurs susceptibles d’affecter les prix de l’immobilier.


##### Tech Stack

Pandas · Numpy · Plotly · LightGBM · MLFlow · Streamlit · Hugging Face · Boto3 · AWS S3
