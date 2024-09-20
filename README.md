# pmb_docker

Pour une installation directe de la version 7.3.18 de pmb :
- Aller dans le répertoire pmb-7.3.18 et télécharger le fichier docker-compose.yml 
- S'identifier sur Docker Hub puis :
    - Télécharger l'image Docker pmb7.3.18-php-apache 
       docker pull denismercier/pmb7.3.18-php-apache
    - Télécharger l'image Docker mariadb:10.6.3
       docker pull mariadb:10.6.3
- Lancer le démon Docker
- Lancer la commande docker-compose up -d --build
- Le serveur pmb est accessible à l'addresse http://localhost.
   
Pour une installation à partir du Dockerfile :
- Aller dans le répertoire pmb-7.3.18 et télécharger le fichier Dockerfile
   Attention ! Le code de pmb n'est pas inclus dans ce repository, il doit être téléchargé à part (cf. COPY dans le fichier Dockerfile).  
