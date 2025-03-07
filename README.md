# Analyse des Fichiers Journaux HTTP avec ELK

## Description du Projet
Ce projet vise à analyser les fichiers journaux des serveurs HTTP Apache en utilisant diverses techniques, notamment les expressions régulières et la stack ELK (Elasticsearch, Logstash, Kibana).

## Objectifs
- Comprendre et comparer les différentes versions du protocole HTTP.
- Configurer un serveur HTTP et créer un client HTTP.
- Gérer les différents formats de fichiers journaux HTTP.
- Analyser les fichiers journaux avec des expressions régulières en Python et R.
- Visualiser les données sous forme de courbes et graphiques.
- Utiliser ELK pour une analyse avancée des journaux.

## Technologies Utilisées
- **Langages** : Python, R
- **Outils** : Logstash, Elasticsearch, Kibana
- **Formats de fichiers journaux** : Apache Access Log, JSON, CSV

## Installation
1. **Prérequis** :
   - Docker et Docker Compose installés
   - Python 3.x installé avec pip
   - R installé si analyse via R
   
2. **Installation de ELK Stack**
   ```bash
   docker-compose up -d
   ```
   
3. **Installation des dépendances Python**
   ```bash
   pip install -r requirements.txt
   ```

## Utilisation
1. **Démarrer le serveur ELK**
   ```bash
   docker-compose up -d
   ```
2. **Exécuter l'analyse avec Python**
   ```bash
   python analyse_logs.py
   ```
3. **Accéder à Kibana**
   - Rendez-vous sur `http://localhost:5601` pour visualiser les journaux analysés.

## Délivrables
- Rapport et annexes du projet
- Archive du projet avec code source et documentation

## Ressources
- [Optimisez la sécurité informatique grâce au monitoring](https://openclassrooms.com/fr/courses/1750566-optimisez-la-securite-informatique-grace-au-monitoring)

## Auteur
- Projet encadré par **Zainab KHALLOUF**
- Contact : zainab.khallouf@univ-ubs.fr

