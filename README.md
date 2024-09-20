# pmb_docker

Pour une installation directe de la version 7.3.18 de pmb :
- Télécharger le fichier docker-compose.yml
- S'identifier sur Docker Hub 
    - Télécharger l'image Docker pmb7.3.18-php-apache 
       docker pull denismercier/pmb7.3.18-php-apache
    - Télécharger l'image Docker mariadb:10.6.3
       docker pull mariadb:10.6.3
- Lancer le démon Docker
- docker-compose up --build 
   
Pour une installation à partir du Dockerfile :
- Télécharger le fichier Dockerfile
   Attention ! Le code de pmb n'est pas inclus dans ce repository, il doit être téléchargé à part (cf. COPY dans le fichier Dockerfile).  
