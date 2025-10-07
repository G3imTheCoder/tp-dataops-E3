# 📋 Planification du Sprint 1 : Pipeline de Performances Scolaires

## 🎯 Sprint Goal

**Mettre en place un pipeline de données fonctionnel capable de télécharger, nettoyer et charger les données de performance scolaire dans PostgreSQL, permettant ainsi la base pour un futur tableau de bord analytique.**

## 📚 Product Backlog - User Stories Priorisées

Voici les User Stories identifiées et leur priorité, issues de notre Product Backlog initial. Les numéros entre parenthèses `(#X)` correspondent aux numéros d'Issue sur GitHub.

| ID  | User Story                                                                                             | Priorité | Issue GitHub |
| :-- | :----------------------------------------------------------------------------------------------------- | :------- | :----------- |
| US1 | En tant que *Data Engineer*, je veux **automatiser le téléchargement Kaggle** pour standardiser la collecte. | Haute    | (#NUMÉRO_ISSUE_US1) |
| US2 | En tant que *Data Analyst*, je veux des **données nettoyées et transformées** pour faciliter l'analyse des performances. | Haute    | (#NUMÉRO_ISSUE_US2) |
| US3 | En tant que *Data Engineer*, je veux **charger les données transformées dans PostgreSQL** pour les rendre accessibles au tableau de bord. | Haute    | (#NUMÉRO_ISSUE_US3) |
| US4 | En tant que *Stakeholder*, je veux un **tableau de bord simple** montrant les performances scolaires pour suivre les tendances. | Moyenne  | (#NUMÉRO_ISSUE_US4) |
| US5 | En tant que *Data Engineer*, je veux une **gestion des erreurs robuste** dans le pipeline pour assurer la fiabilité des données. | Moyenne  | (#NUMÉRO_ISSUE_US5) |

## 🚀 Sprint Backlog (Pour le Sprint 1)

Nous avons sélectionné les User Stories de haute priorité (US1, US2, US3) pour ce sprint d'une semaine. Chaque US a été décomposée en tâches techniques, estimée en Story Points, et attribuée aux membres de l'équipe.
Les numéros entre parenthèses `(#X)` correspondent aux numéros d'Issue sur GitHub.

**Capacité de l'équipe pour le sprint :** Environ 25-30 Story Points (pour un sprint d'une semaine).
**Total des points engagés pour ce sprint :** 30 Story Points.

| Tâche                               | Responsable     | Estimation | Livrable attendu                                                                  | US Associée | Statut (initial) | Issue GitHub |
| :---------------------------------- | :-------------- | :--------- | :-------------------------------------------------------------------------------- | :---------- | :--------------- | :----------- |
| Configurer la clé Kaggle            | Data Engineer   | 2 pts      | Clé Kaggle configurée et accessible sur l'environnement de développement.         | US1         | À faire          | (#NUMÉRO_ISSUE_T1_1) |
| Écrire `extract_from_kaggle()`     | Data Engineer   | 3 pts      | Script Python `extract.py` téléchargeant et extrayant le CSV brut.                | US1         | À faire          | (#NUMÉRO_ISSUE_T1_2) |
| Tester le téléchargement automatique | Data Engineer   | 1 pt       | Fichier CSV brut présent et validé localement.                                    | US1         | À faire          | (#NUMÉRO_ISSUE_T1_3) |
| Analyser le schéma et types         | Data Analyst    | 3 pts      | Document/notes d'analyse du dataset, identification des problèmes de données.     | US2         | À faire          | (#NUMÉRO_ISSUE_T2_1) |
| Définir les règles de nettoyage/transfo | Data Analyst    | 5 pts      | Document/notes détaillant les règles de nettoyage et de transformation.            | US2         | À faire          | (#NUMÉRO_ISSUE_T2_2) |
| Écrire `clean_transform_data()`     | Data Engineer   | 5 pts      | Script Python `transform.py` appliquant les règles de nettoyage/transformation.    | US2         | À faire          | (#NUMÉRO_ISSUE_T2_3) |
| Tester le nettoyage et la transformation | Data Analyst    | 2 pts      | Rapport de validation de la qualité des données transformées.                     | US2         | À faire          | (#NUMÉRO_ISSUE_T2_4) |
| Configurer l'accès DB PostgreSQL    | DevOps Engineer | 2 pts      | Accès testé et fonctionnel à la base de données PostgreSQL.                       | US3         | À faire          | (#NUMÉRO_ISSUE_T3_1) |
| Définir le schéma de table PostgreSQL | Data Engineer   | 3 pts      | Fichier SQL `create_table.sql` pour la table `students_performance`.              | US3         | À faire          | (#NUMÉRO_ISSUE_T3_2) |
| Écrire `load_to_postgresql()`      | Data Engineer   | 3 pts      | Script Python `load.py` chargeant les données transformées dans PostgreSQL.       | US3         | À faire          | (#NUMÉRO_ISSUE_T3_3) |
| Tester le chargement des données    | Data Engineer   | 1 pt       | Vérification de la présence et de l'intégrité des données dans PostgreSQL.        | US3         | À faire          | (#NUMÉRO_ISSUE_T3_4) |
| **Total des points du sprint**      |                 | **30 pts** |                                                                                   |             |                  |              |

## 🗓️ Événements Scrum (Simulation)

### Sprint Planning

*   **Date :** [Date de la simulation - ex: 07 Octobre 2025]
*   **Durée :** 1h
*   **Objectif :** Définir le Sprint Goal et élaborer le Sprint Backlog.
*   **Résultat :** Le Sprint Goal ci-dessus a été défini, et le Sprint Backlog détaillé a été créé et validé par l'équipe.

### Daily Scrum (Exemple pour un jour typique au milieu du sprint)

*   **Date :** [Date de la simulation - ex: 09 Octobre 2025]
*   **Durée :** 15 min
*   **Objectif :** Synchroniser l'équipe, inspecter les progrès et adapter le plan du sprint.
*   **Déroulement simulé :**
    *   **Mehdi Eddalai (Scrum Master) :** "Bonjour l'équipe, commençons notre Daily. Qui veut commencer ?"
    *   **TCHINDE Valdest (Product Owner) :** "Je suis là pour écouter et m'assurer que nous restons alignés sur la valeur."
    *   **[Nom Data Engineer] :** "Hier, j'ai configuré la clé Kaggle (Tâche 1.1 - Terminé) et j'ai bien avancé sur `extract.py` (Tâche 1.2 - En cours). Aujourd'hui, je vise à finaliser `extract.py` et à le tester (Tâche 1.3). Je n'ai pas de bloqueur pour l'instant."
    *   **DONGMO-JIAZET Yann-pavel (Data Analyst) :** "Hier, j'ai terminé l'analyse du schéma des données (Tâche 2.1 - Terminé) et j'ai identifié des valeurs manquantes et des types à convertir. J'ai bien avancé sur la définition des règles de nettoyage (Tâche 2.2 - En cours). Aujourd'hui, je compte finaliser ces règles et les communiquer clairement au Data Engineer. Pas de blocage majeur."
    *   **Ouakrim Mhamed-yasser (DevOps Engineer) :** "Hier, j'ai recherché les meilleures pratiques pour la configuration de la DB. Aujourd'hui, je vais mettre en place l'accès à la base de données PostgreSQL (Tâche 3.1) et m'assurer qu'elle est prête pour le Data Engineer. Je ne vois pas de bloqueurs immédiats."
    *   **TRAORE Mohamed Nour (Data Analyst) :** "En tant que second Data Analyst, j'ai assisté Yann-pavel sur l'analyse et la définition des règles, en me concentrant sur la validation des transformations. Aujourd'hui, je vais aider à peaufiner les règles et préparer les cas de test pour la tâche 2.4. Tout est clair pour moi."
    *   **Mehdi Eddalai (Scrum Master) :** "Excellent, l'avancement est bon. Je note que la tâche 3.1 par Ouakrim sera cruciale pour le Data Engineer ensuite. Je m'assurerai que la communication entre Yann-pavel, Mohamed Nour et le Data Engineer est fluide pour les règles de transformation. Continuons sur cette lancée !"

### Sprint Review

*   **Date :** [Date de la simulation - ex: 11 Octobre 2025]
*   **Durée :** 1h
*   **Objectif :** Inspecter l'incrément réalisé et adapter le Product Backlog si nécessaire.
*   **Résultat simulé :** L'équipe a présenté le pipeline de données "fonctionnel" (même si sans code réel, la description des scripts et des livrables attendus a été faite). Les parties prenantes (simulées) ont validé que le pipeline de base répondait à leurs attentes pour la collecte, le nettoyage et le chargement des données. Des discussions ont eu lieu sur les prochaines étapes, notamment l'intégration avec un outil de tableau de bord.

### Sprint Retrospective

*   **Date :** [Date de la simulation - ex: 11 Octobre 2025 (après la Sprint Review)]
*   **Durée :** 1h
*   **Objectif :** Inspecter l'équipe elle-même et créer un plan d'amélioration pour le prochain sprint.
*   **Résultat simulé :**
    1.  **Ce qui a bien fonctionné :**
        *   "La collaboration et la communication au sein de l'équipe ont été très bonnes, en particulier entre les Data Analysts et le Data Engineer pour les règles de transformation."
        *   "Le Daily Scrum nous a permis de rester alignés et de résoudre rapidement les petites difficultés."
        *   "Le Sprint Goal était clair et a aidé à maintenir le focus de l'équipe."
    2.  **Ce qui aurait pu mieux se passer :**
        *   "L'estimation de 30 Story Points était un peu ambitieuse pour un premier sprint, ce qui a mis une certaine pression sur l'équipe."
        *   "Nous aurions pu anticiper un peu mieux le temps nécessaire à la configuration de l'environnement PostgreSQL."
        *   "La définition des règles de nettoyage aurait pu être plus détaillée dès le début pour réduire les allers-retours."
    3.  **Ce que nous allons améliorer pour le prochain Sprint :**
        *   "Réajuster notre estimation de vélocité pour le prochain sprint, en visant un total de Story Points plus réaliste (ex: 20-25 pts)."
        *   "Organiser une courte session technique en début de sprint pour s'assurer que les environnements de développement et de production (DB) sont prêts et testés."
        *   "Consacrer plus de temps à l'exploration des données et à la documentation détaillée des règles de transformation avant de commencer le développement des scripts."
        *   "Mettre en place un outil de suivi des tâches plus visuel (ex: tableau Kanban) pour mieux visualiser l'avancement."

