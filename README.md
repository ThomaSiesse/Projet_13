# Projet 13 : passer un système IA du POC au MVP et réaliser son portfolio de data engineer

Ce projet a deux volets :

1. **Gestion de projet** : préparer le passage du chatbot RAG du [Projet 11](../Projet_11) d'un POC à un **MVP** déployable dans le cloud, en analysant les besoins, en planifiant, en choisissant l'architecture et en estimant les coûts ;
2. **Portfolio** : présenter les 13 projets réalisés pendant la formation de data engineer.


## Contexte

**Puls-Events** propose une plateforme web pour découvrir et suivre des événements culturels en temps réel. Un POC de chatbot a été réalisé lors du Projet 11. Il repose sur un système **RAG** (Mistral, LangChain, FAISS) alimenté par les événements publics d'OpenAgenda.

L'entreprise veut maintenant transformer ce POC en un **MVP robuste et scalable**.

### Besoins du MVP

- une interface de chatbot conversationnel ;
- une recherche personnalisée pour chaque utilisateur ;
- une **mémoire conversationnelle** (historique et préférences) ;
- une prise en compte du **contexte géographique** selon les préférences de l'utilisateur ;
- une recherche à jour, pour ne manquer aucun événement ;
- un **monitoring** des performances du système ;
- un **déploiement cloud**.

### Utilisateurs cibles

- les utilisateurs actuels de la plateforme, dont la recherche et le confort d'usage seront améliorés ;
- de nouveaux utilisateurs qui cherchent un événement, à court ou à long terme ;
- des profils variés : familles avec de jeunes enfants, amateurs de théâtre, d'opéra, de spectacles…

## Choix du cloud provider

Le comparatif est détaillé dans [comparatif_cloud_mvp.md](comparatif_cloud_mvp.md). AWS, Google Cloud et Azure ont été évalués avec une matrice pondérée :

| Critère | Poids | AWS | Google Cloud | Azure |
| --- | --- | --- | --- | --- |
| Coût de démarrage | 25 % | 4 | 4 | 3 |
| Simplicité et maîtrise de l'équipe | 30 % | 5 | 3 | 3 |
| Services managés suffisants | 15 % | 4 | 4 | 4 |
| Région UE et RGPD | 15 % | 5 | 5 | 5 |
| Portabilité | 15 % | 4 | 4 | 3 |
| **Total pondéré** | 100 % | **4,45** | **3,85** | **3,45** |

**Recommandation : AWS, région Paris (eu-west-3).**

| Besoin | Service retenu |
| --- | --- |
| API du chatbot et pipeline d'ingestion | ECS Fargate |
| Événements et embeddings, avec filtres par ville et par date | RDS PostgreSQL + pgvector |
| Mémoire conversationnelle | DynamoDB ou PostgreSQL |
| Authentification | Cognito |
| Données brutes OpenAgenda | S3 |
| Clés d'API (Mistral) | Secrets Manager |
| Monitoring | CloudWatch, complété par Langfuse pour les appels au LLM |

Google Cloud reste une alternative sérieuse si le coût au repos devient décisif, car Cloud Run peut descendre à zéro instance.

## Contenu du rapport de gestion de projet

Le rapport (`Siesse_Thomas_1_Rapport gestion projet_112026.odt`) suit le plan imposé :

1. **Introduction** : contexte et objectif POC → MVP ;
2. **Analyse des besoins** et des utilisateurs cibles ;
3. **Plan de projet** : jalons, échéancier, livrables (méthode agile) ;
4. **Macro backlog** : fonctionnalités essentielles, priorisées en Must-Have et Nice-to-Have, avec estimation de la complexité, des délais et des risques ;
5. **Architecture technique** : schéma cloud scalable, choix du provider, stratégies de déploiement, de modularité et de monitoring ;
6. **Estimation des coûts** : coût de développement initial (build), coût d'exploitation (OPEX) selon la charge, pistes d'optimisation ;
7. **Bilan** : étapes clés, justification des choix, difficultés rencontrées ;
8. **Annexes** : lien vers le portfolio.

## Portfolio

[Portfolio.md](Portfolio.md) présente les 13 projets de la formation, avec pour chacun le sujet, les compétences, les technologies et le lien vers le dépôt GitHub :

| Domaine | Projets |
| --- | --- |
| Analyse de données | P2 (EdStats), P6 (machine learning, API BentoML) |
| Bases de données SQL | P3 (immobilier), P4 (audit OLAP) |
| NoSQL | P5 (migration MongoDB), P7 (réplication et sharding MongoDB) |
| Pipelines et infrastructure | P8 (Airbyte, dbt, AWS), P9 (Redpanda, PySpark streaming), P10 (Kestra), P12 (Kafka, Debezium, MinIO) |
| IA | P11 (RAG Mistral), P13 (POC → MVP) |


## Auteur

Thomas SIESSE, novembre 2026.
