Structure du Projet
Frontend : Application React construite avec Vite.
Backend : API REST développée en Flask (Python 3.10).
Base de Données : MySQL 5.7.
PHPMyAdmin : Pour l'administration de la base de données.
Nginx : Reverse proxy pour diriger le trafic entre le frontend et le backend.



-Exécuter le Projet :

Étapes
Cloner le Répertoire du Projet :
git clone "https://github.com/azizchouikha/TP-docker.git"
cd todo-app-flask-reactjs

Construire et Démarrer les Conteneurs:
docker-compose up --build

Ouvrez votre navigateur et allez sur http://localhost.(Application Web)
Accédez à http://localhost:8080 pour administrer la base de données.(PHPMyAdmin)

Arrêter les Conteneurs
docker-compose down

Rq:
Variables d'Environnement : Les mots de passe et autres informations sensibles sont définis dans le docker-compose.yml.
Volumes : Le volume db-data assure la persistance des données MySQL.
Réseaux : Le réseau app-network permet aux conteneurs de communiquer entre eux.
