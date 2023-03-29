# Mis en place d'un Api Rest en golang

1. ## Premiere partie : Mise en place de notre structure
- ** Creation de Dokerfile et de docker-compose **

- Dockerfile : 


2. ## Instalation des dépendances

```bash
docker compose run --service-ports web bash 
```
Une fois connecté sur votre conteneur, installer les dependances suivantes: 
```bash
go mod init github.com/prcieux20/monapi
go get github.com/labstack/echo/v4
go get github.com/labstack/echo/v4/middleware@v4.10.2
``` 
- Pour que vos page se recharge automaquiment, installer ce paquet dans votre dockerfile.
puis modifier ceci dans votre fichier toml
inserrer images
```
RUN go install github.com/cosmtrek/air@latest
``` 

