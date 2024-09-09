Système de Recommandation de Vidéos avec Streamlit

Ce projet est une application de système de recommandation de vidéos basée sur les préférences des utilisateurs. L'application est développée avec Streamlit et intègre un processus d'authentification, de sélection des préférences et d'affichage des vidéos recommandées.

Fonctionnalités:

 1. Authentification des Utilisateurs
   - Les utilisateurs peuvent s'inscrire avec un formulaire simple contenant un nom d'utilisateur et un mot de passe.
   - Après l'inscription, les utilisateurs peuvent se connecter pour accéder à l'application.

2. Sélection des Préférences
   - Lors de la première connexion, chaque utilisateur est invité à sélectionner ses préférences de contenu (thématiques des vidéos).
   - Ces préférences sont enregistrées pour personnaliser les recommandations ultérieures.

3. Affichage des Premières Vidéos
   - Après la sélection des préférences, les premières vidéos recommandées sont affichées à l'utilisateur.
   - L'algorithme actuel affiche des vidéos en fonction des préférences choisies et de l'historique des vidéos aimées par l'utilisateur.

Technologies Utilisées

- Python : Langage principal de développement.
- Streamlit : Framework utilisé pour créer l'interface utilisateur de l'application.
- google-api-python-client : Utilisé pour interagir avec l'API YouTube afin de récupérer des vidéos en fonction des préférences.
- pandas : Utilisé pour manipuler les données et enregistrer les préférences dans des fichiers CSV.
- bcrypt: Utilisé pour hacher les mots de passe des utilisateurs.
- Streamlit-authenticator : Module utilisé pour gérer l'inscription et la connexion.

Installation

1. Clonez le dépôt :

   ```bash
   git clone https://github.com/votre-utilisateur/votre-projet.git
   cd votre-projet
   ```

2. Créez et activez un environnement virtuel (optionnel mais recommandé) :

   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Windows: venv\Scripts\activate
   ```

3. Installez les dépendances :

   ```bash
   pip install -r requirements.txt
   ```

4. Lancez l'application Streamlit :

   ```bash
   streamlit run app.py
   ```

Utilisation

1. Inscription : Les nouveaux utilisateurs peuvent créer un compte via un formulaire d'inscription.
2. Connexion : Une fois inscrits, les utilisateurs peuvent se connecter à leur compte pour accéder à l'application.
3. Choix des Préférences : Après la connexion, les utilisateurs sélectionnent leurs préférences de contenu vidéo.
4. Recommandations de Vidéos : Les premières vidéos sont affichées en fonction des préférences de l'utilisateur.

Fonctionnalités Futures

- Intégration complète d'un système de recommandation basé sur le filtrage collaboratif et la similarité cosinus.
- Enregistrement et suivi des interactions des utilisateurs (likes, commentaires, temps de visionnage).
- Affinage des recommandations en fonction des interactions des utilisateurs avec les vidéos.


