# docker-wordpress
# Téléchargez un exemple de fichier docker-compose pour WordPress
git clone https://github.com/kassambara/wordpress-docker-compose
cd wordpress-docker-compose

# Utilisez la commande make pour l'installation automatique et
# configuration de wordpress
make autoinstall

# Ou bien, utilisez les commandes standard de docker-compose
docker-compose up -d --build
docker-compose -f docker-compose.yml -f wp-auto-config.yml run --rm wp-auto-config
Visitez votre site web wordpress à l’adresse http://localhost. Identification par défaut pour admin (http://localhost/wp-login.php):
Username: wordpress
Password: wordpress
Visitez votre base de données via phpMyAdmin à l’adresse http://localhost:8080
Username: root
Password: password
