# 🚀 Projet DataOps : Suivi des Performances Scolaires

## Contexte du Projet

Ce dépôt contient les artefacts de planification et de suivi pour un projet DataOps visant à mettre en place un pipeline automatisé pour le suivi des performances scolaires des étudiants. Ce travail a été réalisé dans le cadre d'un TP simulant un sprint Scrum complet.

## 🎯 Objectif Principal

L'objectif est de construire un pipeline de données automatisé capable de :
1.  **Télécharger** un dataset de performances étudiantes depuis Kaggle.
2.  **Nettoyer et transformer** les données brutes.
3.  **Charger** les données préparées dans une base de données PostgreSQL pour alimenter un futur tableau de bord analytique.

## 📚 Le Dataset

Nous utilisons le dataset "Students Performance Dataset" disponible sur Kaggle :
[https://www.kaggle.com/datasets/rabieelkharoua/students-performance-dataset](https://www.kaggle.com/datasets/rabieelkharoua/students-performance-dataset)

Ce dataset inclut des informations cruciales telles que les scores aux examens, le sexe, l'origine ethnique, le niveau d'éducation des parents, etc., permettant une analyse approfondie des facteurs influençant la réussite scolaire.

## 👥 Composition de l'Équipe

Pour ce sprint, notre équipe est composée comme suit :

|
 Rôle                 
|
 Responsabilité principale                                                                                                    
|
 Membre(s)               
|
|
:-------------------
|
:----------------------------------------------------------------------------------------------------------------------------
|
:----------------------
|
|
**
Product Owner
**
|
 Définit la vision du produit, gère le Product Backlog, maximise la valeur du travail de l'équipe.                              
|
 TCHINDE Valdest         
|
|
**
Scrum Master
**
|
 Facilite le processus Scrum, aide l'équipe à rester concentrée, élimine les obstacles.                                        
|
 Mehdi Eddalai           
|
|
**
Data Engineer
**
|
 Conçoit et construit les pipelines de données, gère l'infrastructure (Kaggle API, PostgreSQL).                                
|
TRAORE Mohamed Nour 
*
|
|
**
Data Analyst
**
|
 Comprend les besoins métier, explore les données, définit les transformations nécessaires pour l'analyse.                      
|
 DONGMO-JIAZET Yann-pavel, Ouakrim Mhamed-yasser   
|
|
**
DevOps Engineer
**
|
 Assurent l'automatisation, la surveillance et le déploiement continu des pipelines . 
|
 
|

## 🗺️ Structure du Dépôt (Vision)

Bien que ce TP se concentre sur la planification, voici la structure envisagée pour le projet final :
Le projet est organisé selon une approche DataOps, structurée en plusieurs étapes : extraction des données depuis Kaggle, préparation et nettoyage, analyse exploratoire, visualisation des résultats, puis définition du pipeline automatisé.
Chaque étape correspond à une User Story suivie dans GitHub Projects pour assurer une gestion agile et collaborative du cycle de vie des données.
