# Portfolio Data Engineer - SIESSE Thomas

Data engineer spécialisé dans l'orchestration des flux de données, de la base de données à l'infrastructure cloud, avec la mise en place de nettoyage de données, de pipelines de données, de systèmes NLP et RAG.
Je conçois, construis, teste et industrialise des systèmes de données, du traitement brut jusqu'au produit déployé.

## Résumé

Ce portfolio regroupe l'ensemble de mes 13 projets réalisés pendant ma formation. Mon parcours m'a permis de couvrir l'ensemble des processus de traitement des données : analyse de données, pipelines d'orchestration de flux, création de bases de données.

## Vue d'ensemble des projets

| N° Projet | Projet | Compétences | Technologie |
| ---------- | ------------------------------------------------------- | ------------------------------------------------------------------------------ | --------------------------------------------------------------- |
| Projet_1 | Découvrez votre formation de data engineer | Mise en place | |
| Projet_2 | Analysez les données de systèmes éducatifs | Analyses statistiques descriptives | Python, Jupyter, NumPy, Seaborn, Matplotlib |
| Projet_3 | Traitement SQL et création d'une BDD | Modélisation d'une base de données | SQL, Modélisation |
| Projet_4 | Audit d'un environnement de données | Audit et identification d'erreurs | SQL, Analyse de logs |
| Projet_5 | Maintenance, documentation et sécurisation d'une BDD | Base de données non structurées et Docker | MongoDB, Docker, AWS, CRUD |
| Projet_6 | Analyse de consommation de bâtiments | Machine learning et déploiement dans le cloud | BentoML, AWS ECS, Pydantic |
| Projet_7 | Conception d'une BDD NoSQL | Architecture de collecte et stockage des données | MongoDB, Polars, Tableau |
| Projet_8 | Conception d'une infrastructure de données | Pipeline ELT et schéma d'architecture | dbt-DuckDB, PostgreSQL, Airbyte, AWS, draw.io |
| Projet_9 | Modélisation d'une infrastructure dans le cloud (AWS) | Pipeline ETL en streaming | Redpanda, PySpark, Docker, Python |
| Projet_10 | Mise en place d'un pipeline d'orchestration de flux | Orchestration de flux et monitoring | Kestra, Docker, Python, DuckDB |
| Projet_11 | Conception d'un système RAG | Intégration de modèle NLP dans un système RAG (POC) | LangChain, FAISS, Mistral AI |
| Projet_12 | Gestion d'un projet d'infrastructure | Pipeline ETL CI/CD | PostgreSQL, Debezium, Kafka, MinIO, dbt-DuckDB, Tableau, Python |
| Projet_13 | Passage du POC au MVP | Pilotage de projet agile, estimation des coûts et communication professionnelle | Méthode agile, méthodologie en V |

## Détail des projets

### Projet_1 - Découvrez votre formation de Data Engineer

Définition du périmètre de la formation, découverte du mentor, planification des sessions de mentorat et mise en place des outils collaboratifs.

***Compétences*** : définir un objectif professionnel, planifier.

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_1](https://github.com/ThomaSiesse/Projet_1)

### Projet_2 - Analysez les données de systèmes éducatifs

Analyse exploratoire du jeu de données **EdStats** de la Banque mondiale (indicateurs sur l'éducation dans le monde). Le but est de décrire les fichiers, de mesurer leur qualité (doublons, valeurs manquantes, colonnes vides) et de les nettoyer pour garder les informations utiles.

***Compétences*** : analyses statistiques descriptives, Python

***Technologie*** : Python, SQL, Jupyter Notebook, Pandas, NumPy

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_2](https://github.com/ThomaSiesse/Projet_2)

### Projet_3 - Entraînez-vous avec SQL et créez votre BDD

Création d'une base de données relationnelle à partir des transactions immobilières françaises du 1er semestre 2020, puis analyse du marché avec des requêtes SQL.

***Compétences*** : audit et identification d'erreurs, analyse d'un jeu de données

***Technologie*** : SQL, Modélisation, MySQL

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_3](https://github.com/ThomaSiesse/Projet_3)

### Projet_4 - Auditez un environnement de données

Audit de la base de données décisionnelle (OLAP) de **SuperSmartMarket**, une chaîne française de supermarchés. Le but est de comprendre pourquoi le chiffre d'affaires affiché dans Power BI change le lendemain.

***Compétences*** : bases de données non structurées, schéma en étoile, Docker, cycle de vie des données

***Technologie*** : SQL, analyse de logs, PostgreSQL

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_4](https://github.com/ThomaSiesse/Projet_4)

### Projet_5 - Maintenez et documentez un système de stockage des données sécurisé et performant

Ce projet migre un jeu de données médicales vers **MongoDB** de façon automatisée et sécurisée, avec un test de conformité des données. Le fichier source est un CSV de **55 500 dossiers patients**. Une étude de déploiement dans le cloud AWS a été réalisée.

***Compétences*** : bases de données non structurées et Docker

***Technologie*** : BentoML, AWS ECS, Pydantic

***Dépôt GitHub*** : [github.com/ThomaSiesse/Project_5](https://github.com/ThomaSiesse/Project_5)

### Projet_6 - Anticipez les besoins en consommation de bâtiments

Ce projet se base sur le machine learning pour prédire les émissions de CO₂ des bâtiments non résidentiels de Seattle à partir de leurs caractéristiques structurelles. Le modèle est exposé par une API REST (BentoML) déployée sur AWS.

***Compétences*** : machine learning, déploiement dans le cloud, feature engineering

***Technologie*** : Python, SQL, Jupyter Notebook, Pandas, NumPy, scikit-learn

***Dépôt GitHub*** : [github.com/ThomaSiesse/Anticipez-les-besoins-en-consommation-de-batiments](https://github.com/ThomaSiesse/Anticipez-les-besoins-en-consommation-de-batiments)

### Projet_7 - Concevez et analysez une base de données NoSQL

Restauration et analyse d'une base **MongoDB** d'annonces de locations de courte durée (Airbnb) à Paris et à Lyon, puis mise en place d'une architecture distribuée (réplication et sharding) pour pérenniser la base.

***Compétences*** : architecture de collecte et stockage des données

***Technologie*** : MongoDB, Polars, Tableau

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_7](https://github.com/ThomaSiesse/Projet_7)

### Projet_8 - Construisez et testez une infrastructure de données

Pipeline ELT de données météo, de l'ingestion multi-sources jusqu'à un entrepôt de données testé, documenté et déployé sur AWS. Les données sont transformées avec dbt-DuckDB et orchestrées par Airbyte.

***Compétences*** : pipeline ELT et schéma d'architecture

***Technologie*** : dbt-DuckDB, PostgreSQL, Airbyte, AWS, draw.io

***Dépôt GitHub*** : [github.com/ThomaSiesse/projet8](https://github.com/ThomaSiesse/projet8)

### Projet_9 - Modélisez une infrastructure dans le cloud

Conception d'une infrastructure hybride **on-premise / AWS** pour InduTechData, et POC d'un pipeline de données en temps réel avec **Redpanda** et **PySpark Structured Streaming**, entièrement conteneurisé avec Docker.

***Compétences*** : pipeline ETL en streaming

***Technologie*** : Redpanda, PySpark, Docker, Python

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_9](https://github.com/ThomaSiesse/Projet_9)

### Projet_10 - Mettez en place un pipeline d'orchestration des flux

Pipeline **Kestra** + **DuckDB** qui automatise chaque mois, pour le caviste BottleNeck :

- le nettoyage et la fusion des données ERP et du site web ;
- le calcul du chiffre d'affaires ;
- la segmentation des vins en premium et ordinaires.

***Compétences*** : orchestration de flux et monitoring

***Technologie*** : Kestra, Docker, Python, DuckDB

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_10](https://github.com/ThomaSiesse/Projet_10)

### Projet_11 - Concevez et déployez un système RAG

Ce projet implémente un assistant virtuel de recommandation d'événements culturels à Marseille, basé sur les modèles Mistral et la technique de Retrieval-Augmented Generation (RAG). Il répond aux demandes en langage naturel à partir des événements publics OpenAgenda, sans jamais inventer d'événement.

***Compétences*** : intégration de modèle NLP dans un système RAG (POC)

***Technologie*** : LangChain, FAISS, Mistral AI

***Dépôt GitHub*** : [github.com/ThomaSiesse/projet-11-RAG](https://github.com/ThomaSiesse/projet-11-RAG)

### Projet_12 - Gérez un projet d'infrastructure

Pipeline de données qui calcule les avantages accordés aux salariés sportifs. Des consumers lisent les topics Kafka pour déclencher le nettoyage des données. Elles sont d'une part envoyées vers Slack sous forme de messages de félicitation, et d'autre part stockées dans une BDD MinIO, puis transformées par un traitement en médaillon avec dbt-DuckDB pour être exploitées via Tableau.

***Compétences*** : pipeline ETL CI/CD

***Technologie*** : PostgreSQL, Debezium, Kafka, MinIO, dbt-DuckDB, Tableau, Python

***Dépôt GitHub*** : [github.com/ThomaSiesse/POC_avantages_sportifs](https://github.com/ThomaSiesse/POC_avantages_sportifs)

### Projet_13 - Passez votre système IA du POC au MVP et réalisez votre portfolio de Data Engineer

Réalisation d'un rapport de gestion de projet avec la méthode agile pour préparer le passage du POC du Projet_11 vers un MVP. Analyse des besoins, définition d'une architecture cloud et choix d'un cloud provider, estimation des coûts de build et d'OPEX.

***Compétences*** : pilotage de projet agile, estimation des coûts et communication professionnelle

***Technologie*** : méthode agile, méthodologie en V

***Dépôt GitHub*** : [github.com/ThomaSiesse/Projet_13](https://github.com/ThomaSiesse/Projet_13)

## Compétence globale

Je maîtrise la chaîne de traitement des données, de l'ingestion à la mise à disposition de données nettoyées et exploitables. Mes projets couvrent l'ensemble du cycle :

- **Collecte et ingestion** : extraction depuis des sources multiples (bases SQL, fichiers CSV, API, flux Kafka et Debezium) avec Airbyte, Kafka et Redpanda.
- **Nettoyage et qualité** : détection des doublons, valeurs manquantes et erreurs, tests de conformité et audit d'environnements de données.
- **Modélisation et stockage** : conception de bases relationnelles (PostgreSQL, MySQL) et non structurées (MongoDB), schémas en étoile, architectures distribuées (réplication, sharding) et stockage objet (MinIO).
- **Transformation et orchestration** : pipelines ETL et ELT avec dbt-DuckDB, orchestration avec Kestra et monitoring, traitement en streaming avec PySpark.
- **Infrastructure et déploiement** : conteneurisation avec Docker, déploiement sur AWS (ECS, services cloud), intégration CI/CD et conception d'architectures hybrides.
- **Machine learning et IA** : modèles de prédiction exposés par API REST (BentoML), intégration de modèles NLP dans un système RAG avec LangChain, FAISS et Mistral AI.
- **Restitution et pilotage** : visualisation avec Tableau, documentation technique, schémas d'architecture et gestion de projet agile avec estimation des coûts.

## Contact

GitHub : [github.com/ThomaSiesse](https://github.com/ThomaSiesse)

LinkedIn : [linkedin.com/in/thomas-siesse-b71a39194](https://www.linkedin.com/in/thomas-siesse-b71a39194/)

Email : siesse.thomas@gmail.com
