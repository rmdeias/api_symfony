### Etape 1 ###
#### a faire la première fois ####
docker builder prune
docker system prune
docker rm [containerID]

dans ./ sudo docker-compose build (pour construire les containers)

### Etape 2 ###

sudo docker-compose up -d (pour monter les containers)

sudo docker ps (pour vérifier la présence des 3 cointainers mysql, nginx, php)

### Etape 3 ###
sudo docker exec -it {NomDuContainerPhp} /bin/bash (pour rentrer dans le container)

### Etape 4 ###

composer create-project symfony/skeleton api 6.0.* (création du projet symfony)


### Etape 5 ###
cd api
symfony server:start

### Etape 6 ###

sortir du server symfony  Ctrl + C  ou symfony server:stop

exit (pour sortir du container php)

sudo docker-compose stop (pour arreter les containers)
