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

# Fondamentaux de l'Ingénierie des Données (Data Engineering)

N.B : Il s'agit uniquement des fondamentaux de l'ingénierie des données à connaître pour pouvoir bien suivre ce Projet. En aucun cas, je ne prétends vous donner ici toutes les notions fondamentales de la Data Engineering. Si le sujet vous intéresse, vous trouverez beeaucoup d'autres ressources adaptées sur Internet.

## Comprendre le Concept de Data Warehouse

- The challenges are always about moving data from the data source to other environments so the business can use it to get information.

- Data warehouses were first developed in the 1980s to transform data from operational systems to decision-making support systems. The key principle of a data warehouse is combining data from many different sources into a single location and then transforming it into a format the data warehouse can process and store.

- Data Silos have always occurred in large organizations. This is quite common in large organizations where each department has different goals, responsibilities, and priorities. So Data Data comes from many different source systems.

- To get the full benefit of the data, we need to store the data from different systems in one central place or storage.

- Data warehouse products are mostly able to store and process data seamlessly and the user can use the SQL language to access the data in tables with a structured schema format.

- In this Project-based course, we will use BigQuery as Data Warehouse. We'll talk more about BigQuery in a future lesson.

## Différence entre ETL et ELT

# Commencez avec Google Cloud Platfor (GCP)

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




# Building ELT Pipeline (Data Engineering)

# Data Analysis and Visualization (Data Analyst/Business Analyst)

# Building Machine Learning Models with BigQueryML
