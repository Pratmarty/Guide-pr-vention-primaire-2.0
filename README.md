# Application de Dépistage de la Fragilité Motrice en Maison de Retraite v2.0

[cite_start]Cette application Streamlit simule un dépistage de la fragilité motrice chez les personnes de 65 ans et plus à leur arrivée en maison de retraite. Elle est basée sur le "Guide Prévention primaire : Dépistage par les kinésithérapeutes de la fragilité motrice par un score fonctionnel chez les personnes de 65 ans et plus, vivant à domicile" de l'Ordre des Masseurs-Kinésithérapeutes (Juin 2022).

**⚠️ AVERTISSEMENT IMPORTANT :**
Cette application est une **démonstration conceptuelle à des fins éducatives uniquement**.A ETE CREE PAR ADRIEN PRATMARTY DANS LE CADRE DE DON MEMOIRE Elle **ne remplace pas une évaluation clinique professionnelle** par un médecin, un gériatre ou un kinésithérapeute. Elle ne doit en aucun cas être utilisée pour prendre des décisions médicales ou de prise en charge réelles. Consultez toujours un professionnel de la santé qualifié pour une évaluation complète et des conseils personnalisés.

## Fonctionnalités

* **Informations Patient et Évaluation :** Saisie du nom, de l'âge, du sexe et de la date d'évaluation.
* **Interrogatoire :** Questions clés sur les antécédents de chutes, la peur de chuter, les douleurs chroniques, les troubles cognitifs et la prise de médicaments.
* **Tests Fonctionnels :** Entrée des résultats de tests standards (Appui Unipodal, Timed Up and Go, Lever de Chaise, Vitesse de Marche, Grip Test), ainsi que des observations sur la difficulté à se relever du sol et les anomalies orthopédiques.
* **Analyse de Fragilité Simulé :** Calcul d'un score de fragilité et détermination d'un niveau de fragilité (Non fragile, Pré-fragile, Fragile) basé sur les critères du guide.
* **Visualisation "Ce qui va/ne va pas" :** Un graphique radar montrant les points forts et faibles de la personne par rapport aux seuils de risque, sur une échelle de 0 (idéal) à 5 (très problématique).
* **Recommandations Ciblées :** Suggestions adaptées au niveau de fragilité et aux facteurs de risque identifiés, incluant l'orientation vers des professionnels de santé.
* **Historique des Évaluations :** Affichage de toutes les évaluations réalisées pendant la session en cours du navigateur.
* **Export JSON de l'Historique :** Possibilité de télécharger l'historique de la session au format JSON pour une sauvegarde manuelle.
* **Export PDF (Suggestion) :** Instructions pour utiliser la fonction d'impression du navigateur pour générer un PDF du rapport.

## Comment l'exécuter localement

1.  **Pré-requis :** Assurez-vous d'avoir [Python](https://www.python.org/downloads/) installé sur votre machine (version 3.8 ou supérieure recommandée).

2.  **Cloner le dépôt GitHub (ou télécharger les fichiers) :**
    Si vous avez Git, ouvrez votre terminal et exécutez :
    ```bash
    git clone <URL_de_votre_dépôt>
    cd <nom_de_votre_dépôt>
    ```
    Sinon, téléchargez les fichiers `streamlit_app.py`, `requirements.txt` et `README.md` dans un même dossier.

3.  **Créer un environnement virtuel (recommandé) :**
    ```bash
    python -m venv venv
    # Sur Windows
    .\venv\Scripts\activate
    # Sur macOS/Linux
    source venv/bin/activate
    ```

4.  **Installer les dépendances :**
    Avec l'environnement virtuel activé, installez les bibliothèques nécessaires :
    ```bash
    pip install -r requirements.txt
    ```

5.  **Exécuter l'application Streamlit :**
    ```bash
    streamlit run streamlit_app.py
    ```
    Ceci ouvrira l'application dans votre navigateur web par défaut.

## Déploiement sur Streamlit Community Cloud

Vous pouvez facilement déployer cette application sur [Streamlit Community Cloud](https://streamlit.io/cloud). Voici les étapes générales :

1.  **Créer un dépôt GitHub :** Assurez-vous que tous les fichiers (`streamlit_app.py`, `requirements.txt`, `README.md`) sont dans un dépôt GitHub public.
2.  **Se connecter à Streamlit Community Cloud :** Allez sur `share.streamlit.io` et connectez-vous avec votre compte GitHub.
3.  **Déployer une nouvelle application :** Cliquez sur "New app" ou "Deploy an app".
4.  **Sélectionner le dépôt :** Choisissez votre dépôt GitHub, la branche (généralement `main` ou `master`), et le fichier principal de l'application (qui est `streamlit_app.py`).
5.  **Déployer !** Streamlit Cloud construira et déploiera automatiquement votre application. Il utilisera `requirements.txt` pour installer les dépendances.

L'application sera ensuite accessible via une URL publique (par exemple, `votre-utilisateur.streamlit.app/votre-app`).

## Référence Scientifique (source principale d'inspiration)

* Ordre des masseurs-kinésithérapeutes. (Juin 2022). [cite_start]*Guide Prévention primaire : Dépistage par les kinésithérapeutes de la fragilité motrice par un score fonctionnel chez les personnes de 65 ans et plus, vivant à domicile*.
