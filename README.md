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

à l'issue de ces opérations, vous aurez la libraire python nécessaire pour l'execution des projets :

- Speed Dating : [https://github.com/pradelf/speeddating](https://github.com/pradelf/speeddating)
- Kayak : [https://github.com/pradelf/kayak](https://github.com/pradelf/kayak)
- Conversion Challenge : [https://github.com/pradelf/conversion-rate-challenge](https://github.com/pradelf/conversion-rate-challenge)
- Uber Pickups : [https://github.com/pradelf/uberpickups](https://github.com/pradelf/uberpickups)
- Get Around : [https://github.com/pradelf/getaround](https://github.com/pradelf/getaround)]
- Wall Mart Sales :
- ATT : [https://github.com/pradelf/att](<https://github.com/pradelf/att>)
- OASIS (projet collectif) :

Le projet [Steam](https://github.com/pradelf/steam) est particulier car il est nécessaire de la faire executer dans l'environnement [Databricks](https://www.databricks.com/fr)
si vous voulez exporter les dépendances des projets, vous pouvez utiliser la commande :

```bash
pip freeze -l git+https://github.com/pradelf/fpcia.git@6d2560ca7e97f6aa67a97c89445da45907015b30#egg=fpcia
```

Vous pouvez vérifer votre environnement local d'évaluation avec la commande ```pip config list -v``` qui vous donne votre configuration local de recherche de Python et des librairies utilisées.

##  💾 Projets de Data Science & Machine Learning

###  🧱 1. Construction et mise en place d’une infrastructure de gestion de données

#### Kayak

Extraction automatisée des informations sur les hôtels et la météo pour une liste donnée de villes
Stockage des données nettoyées dans AWS S3, puis transfert vers une base AWS RDS
Requêtes SQL pour sélectionner les meilleures villes selon les conditions météo
Génération de cartes interactives illustrant les températures quotidiennes et les gammes de prix des hôtels.

##### Tech Stack

APIs · BeautifulSoup · Boto3 · AWS S3 · AWS RDS · SQL · SQLAlchemy · Plotly

### 🔍 2. Analyse exploratoire de données (EDA)

####  Speed Dating

- Exploration d’un jeu de données de speed dating
- Identification des facteurs influençant la probabilité d’obtenir un second rendez-vous.

#####  Tech Stack

Pandas · Numpy · Seaborn · Matplotlib

### 🤖 3. Analyse prédictive de données structurées (IA & Machine Learning)

#### Conversion Challenge

- Modélisation du taux de conversion d’une newsletter à partir de variables déséquilibrées

#### Walmart

- Estimation des ventes hebdomadaires des magasins
- Interprétation des indicateurs économiques pour planifier les campagnes marketing

####  Uber

- Optimisation du temps d’attente des clients
- Création d’algorithmes de détection de zones chaudes (hot-zones) selon l’heure de la journée

##### Tech Stack

Scikit-learn · XGBoost · Régression linéaire / logistique · Arbres de décision · Forêts aléatoires · Boosting · GridSearch · Validation croisée · K-Means · DBSCAN · Mélange gaussien · KNN

### 💬 4. Analyse prédictive de données non structurées

#### AT&T Spam Detector

- Développement d’un modèle de deep learning détectant automatiquement les spams selon le contenu textuel
- Traitement complet du langage naturel (NLP) : tokenisation, lemmatisation, encodage, embedding

##### Tech Stack

Tensorflow · PyTorch · Transformers · NLP
