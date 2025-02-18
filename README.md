## Business Questions

These questions focus on trends, seasonality, and long-term insights, emphasizing why analyzing multiple months of data is crucial.  

### **Market Demand & Seasonality**  
1. **How does the demand for yellow taxis fluctuate over time (daily, weekly, monthly, and seasonally)?**  
2. **What are the peak hours for yellow taxi trips in different boroughs and zones?**  
3. **How do weather conditions or major events (holidays, sports events) impact yellow taxi usage over time?**  

### **Customer Behavior & Ride Characteristics**  
4. **What are the most popular pickup and drop-off locations, and how do they change over time?**  
5. **What is the average trip distance, and how does it vary by borough, time of day, and season?**  
6. **How many trips have only one passenger versus multiple passengers, and does this change seasonally?**  

### **Financial & Pricing Analysis**  
7. **How does the total fare revenue of yellow taxis change over time?**  
8. **What is the average fare per trip, and how does it vary by borough, time of day, and trip distance?**  
9. **What is the proportion of different payment types (credit card, cash, etc.), and has it changed over time?**  
10. **How often do passengers tip, and what factors (time of day, borough, fare amount) influence tip amounts?**  
11. **How much revenue is generated from additional charges (MTA tax, congestion surcharge, airport fees), and has it changed over time?**  

### **Competitive Insights & Operational Efficiency**  
12. **Which boroughs or zones have the highest and lowest trip volumes, and how do they compare over time?**  
13. **How frequently do yellow taxis serve airports (JFK, LaGuardia, Newark), and what is the average fare for these trips?**  
14. **How often do taxis use different rate codes (e.g., standard rate vs. negotiated fares), and how do these rates vary across boroughs?**  
15. **How long do trips typically take, and is there a trend of increasing or decreasing trip durations over time?**  

These insights will help you understand market demand, customer behavior, and financial trends, providing a solid foundation for competing against yellow taxis in NYC.

# Vidéo présentation du Cours (une sorte de page de garde)

# Section 0 : Bienvenue dans ce cours

## Vidéo : Introduction - Présentation du Scénario

## Notes importantes pour les étudiant(e)s (texte)

- Ressources : Comment les télécharger et les utiliser

- Détail des Questions Business

# Section 1 : Fondamentaux de l'Ingénierie des Données (Data Engineering)

N.B : Il s'agit uniquement des fondamentaux de l'ingénierie des données à connaître pour pouvoir bien suivre ce Projet. En aucun cas, je ne prétends vous donner ici toutes les notions fondamentales de la Data Engineering. Si le sujet vous intéresse, vous trouverez beeaucoup d'autres ressources adaptées sur Internet.

## Texte : Comprendre le Concept de Data Warehouse

Dans le monde des données, un des défis majeurs est de déplacer les données depuis leurs sources vers d'autres environnements afin qu'elles puissent être exploitées pour générer de l'information utile aux décisions stratégiques. C'est ici qu'intervient le **Data Warehouse**.  

#### **Origine et Objectif du Data Warehouse**  
Les Data Warehouses ont été développés dans les années 1980 pour répondre à un besoin croissant : transformer les données issues des systèmes opérationnels en un outil puissant d'aide à la décision. Le principe clé d’un Data Warehouse est de **rassembler les données provenant de sources multiples en un seul endroit**, puis de les **transformer et structurer** afin qu’elles puissent être stockées et exploitées efficacement.  

#### **Les Problèmes de Silos de Données**  
Dans les grandes organisations, il est très courant de voir apparaître des **silos de données**. Chaque département (Finance, Marketing, Ressources Humaines, etc.) travaille souvent avec ses propres systèmes et bases de données, car ils ont des objectifs et des priorités différentes. Cela entraîne une dispersion des données et rend difficile leur exploitation pour une analyse globale et cohérente.  

#### **Pourquoi un Data Warehouse ?**  
Afin de maximiser la valeur des données, il est essentiel de **les centraliser** dans un **espace unique**, un Data Warehouse. Cela permet de :  
✅ **Briser les silos de données** et faciliter leur accès.  
✅ **Fournir une vue unifiée** des données à travers toute l’organisation.  
✅ **Améliorer la qualité des analyses et la prise de décision** grâce à une structuration optimisée des données.  

#### **Comment fonctionne un Data Warehouse ?**  
Les solutions de Data Warehouse sont conçues pour stocker et traiter de grandes quantités de données de manière efficace. Les utilisateurs peuvent accéder aux données via des **requêtes SQL**, qui permettent d’interroger les tables selon une structure bien définie. Cela facilite l’analyse et la production de rapports détaillés à partir des données centralisées.  

#### **Le Data Warehouse dans ce cours**  
Dans ce cours, nous allons utiliser **Google BigQuery** comme Data Warehouse. BigQuery est une solution cloud qui offre de puissantes capacités de stockage et d’analyse de données à grande échelle. Nous explorerons en détail son fonctionnement et ses avantages dans une leçon dédiée.  

📌 **Récapitulatif : Pourquoi utiliser un Data Warehouse ?**  
✅ Centralisation des données pour une meilleure accessibilité.  
✅ Amélioration des performances d’analyse et de requêtage.  
✅ Suppression des silos pour une vision globale des données.  
✅ Facilité d’utilisation grâce au langage SQL.  

## Vidéo : Différence entre ETL et ELT

### **Définition de l'ETL** 
**Extract – Transform – Load**  
1. **Extract** : Extraction des données depuis plusieurs sources.  
2. **Transform** : Transformation avant le stockage (nettoyage, agrégation, jointures).  
3. **Load** : Chargement des données transformées dans l'entrepôt de données (Data Warehouse).  

---

### **Définition de l'ELT**  
**Extract – Load – Transform**  
1. **Extract** : Extraction des données brutes depuis plusieurs sources.  
2. **Load** : Chargement des données brutes directement dans un Data Warehouse ou Data Lake.  
3. **Transform** : Transformation directement dans le stockage (via SQL, Spark, BigQuery, Snowflake).  

---

### **Différences clés entre ETL et ELT**  
| Critère         | ETL                          | ELT                          |
|----------------|-----------------------------|-----------------------------|
| **Quand ?**     | Avant le stockage           | Après le stockage           |
| **Où ?**       | Serveur ETL                  | Data Warehouse / Data Lake  |
| **Performance** | Plus lent (serveurs limités) | Plus rapide (scalabilité du cloud) |
| **Flexibilité** | Structuré                    | Adapté au Big Data          |
| **Stockage**   | Seulement les données utiles | Toutes les données brutes   |

---

### **Conclusion**  
- L’**ETL** est adapté aux systèmes traditionnels nécessitant des données transformées avant stockage.  
- L’**ELT** est plus efficace pour les architectures cloud, exploitant la puissance de calcul des entrepôts modernes.  
- Le choix dépend du contexte, de l’infrastructure et du volume des données.  


# Section 2 : Commencez avec Google Cloud Platform (GCP)

## Création d'un compte GCP

Le processus d'inscription à GCP est très facile. Il suffit de suivre ces étapes :

- Accédez à GCP console (nterface graphique de GCP) en allant sur https://console.cloud.google.com/ via n'importe quel navigateur web

- Connectez-vous avec votre compte Google (par exemple, Gmail).

- Inscrivez-vous à GCP en utilisant votre compte Google.

N.B : Lors de l'inscription, il vous sera demandé de renseigner un moyen de paiement, par exemple une carte bancaire. Mais rasurez-vous, rien ne vous sera facturé à ce stade.

De plus, si c'est otre première inscription, vous aurez droit à un crédit de 300$ à consommer en 90 jours (3 mois). Avec ce crédit, vous pouvez essayer n'importe quel service de GCP dans les 90 jours.

## Exploration de GCP console et création d'un Projet

- Créer un Projet

- Epingler les services suivants pour pouvoir vite y accéder : IAM & Admin, Cloud Storage, BigQuery, Composer, Vertex AI, Looker Studio. Nous n'utiliserons pas les deux derniers dans cette formation mais j'en parlerai brièvement.

- Utilisation de Cloud Shell et Cloud Editor : Tapez par exemple *ls* dans Cloud Shell et exécutez le cote *print("Hello world") dans Cloud Editor avec python3 hello_world.py

## Présentation des services GCP que nous utiliserons dans ce cours

Les Services du domaine "Analytics" :

- Cloud Composer: Un service géré (*Managed Service*) pour Airflow. Airflow est un outil d'orchestration de tâches basé sur Python.

- Dataproc: Un service géré pour Hadoop qui inclut HDFS, MapReduce, Spark, Presto, et bien plus encore. (On ne l'utilisera pas particulièrement dans cette formation mais c'est un important outil pour un Data Engineer travaillant dans GCP)

- Looker Studio: Un outil simple de visualisation pour visualiser les données. A ne pas confondre avec Looker qui est un outil BI complet pour visualiser les données dans des rapports et des tableaux de bord.

- BigQuery: Un service d'entrepôt de données sans serveur (*A serverless data warehouse service*)

- etc.

Les Services du domaine "Storage" :

- Cloud Storage : Un stockage d'objets sans serveur pour stocker des fichiers volumineux. Il est souvent utilisé comme un Data Lake.

- etc.

Les Services du domaine "Management"

- IAM & Admin: Gestion des utilisateurs et des projets pour tous les services GCP

- etc.

Les Services du domaine "Artificial Intelligence"

- Vertex AI : comporte tous les outils dont vous avez besoin pour créer du machine learning et du MLOps – par exemple, des notebooks, des pipelines, un magasin de modèles et d'autres services liés au machine learning




# Section 3 : Extraction des données depuis la source vers Google Cloud Storage

## Vidéo : Clonage du répertoire GitHub et installation des dépendances dans Cloud Shell

Bienvenue dans cette leçon où il s'agira de :

- cloner le répertoire github du projet dans le Cloud Shell
- Créer et activer un environnement virtuel Python
- d'installer les packages nécessaires.

## Vidéo : Création d’un Bucket GCS et upload du projet

Bienvenue dans cette leçon où il s'agira de :

- Créer un Bucket GCS (Console GCP)

- Uploader le répertoire du projet dans ce Bucket (Cloud Shell)

***export DESTINATION_BUCKET_NAME=yellow-taxi-trips-analytics-data-bucket***

***gcloud storage cp -r nyc-yellow-taxi-trips/* gs://$DESTINATION_BUCKET_NAME/from-git/***


## Video : Exploration des données source et réflexion sur l'automatisation du téléchargement des fichiers parquet

## Video : Limites du script simple et améliorations dans le Script optimisé pour un Pipeline en production

## Vidéo : Implémentation et exécution du script optimisé pour l'extraction des données vers GCS

## Leçon Texte : **Conclusion : Extraction des données vers Google Cloud Storage**

### **Slide 1 : Titre & Introduction**
- **Titre : Fin de la phase d’Extraction - Passage à l’étape suivante**
- **Sous-titre : Centralisation des données dans BigQuery**
- Image d’illustration : Pipeline de données avec une flèche vers BigQuery

---

### **Slide 2 : Récapitulatif de la phase d’Extraction**
✅ **Nous avons réalisé :**
- **Clonage du répertoire GitHub et installation des dépendances**
- **Création d’un Bucket GCS et upload du projet**
- **Exploration des données source et réflexion sur leur automatisation**
- **Identification des limites d’un script simple**
- **Implémentation et exécution d’un script optimisé pour l’extraction des fichiers PARQUET vers GCS**

---

### **Slide 3 : Importance de cette étape**
📌 **Pourquoi cette phase est cruciale ?**
- Permet de **collecter les données brutes** dans un espace de stockage centralisé (GCS).
- Assure un **pipeline robuste et automatisé** pour l’ingestion des fichiers.
- Pose les bases pour l’étape suivante : **le chargement des données dans BigQuery.**

---

### **Slide 4 : Prochaine étape - Centralisation des données dans BigQuery**
🚀 **Phase suivante : Le chargement des données dans BigQuery (Load)**
- Objectif : **Transférer les données brutes de GCS vers BigQuery** pour les rendre exploitables.
- Permet d’avoir **une seule source de vérité** pour toutes les analyses.
- Déploiement d’un processus **scalable et optimisé pour le Cloud.**

📌 **Ce que nous allons voir :**
✅ Création des tables BigQuery
✅ Chargement des fichiers PARQUET depuis GCS
✅ Automatisation du processus avec Cloud Composer

---

### **Slide 5 : Conclusion & Transition**
🎯 **Félicitations !** Vous avez terminé la phase d’extraction des données.

📢 **Dans la prochaine section, nous verrons comment charger ces données dans BigQuery pour centraliser l’information et faciliter les analyses.**

🔜 **Passons maintenant à la phase Load !** 🚀


# Section 4 : Chargement des données brutes de GCS vers BigQuery pour les rendre exploitables



# Section 5 : Data Analysis and Visualization (Data Analyst/Business Analyst)

# Section 6 : Building Machine Learning Models with BigQueryML

## Qu'est-ce que BigQuery ML ?

## Démo : Construire et évaluer des Modèles ML pour prédire le prix d'un trajet en taxi jaune à New Yoork
