Keycloak theme customization
============================

This repo shows how to customize Keycloak theme.
See keycloak reference for additional documentation.

# Build the docker image
docker build -t my-keycloak-image .

# Start
```
docker-compose up
```

# Access keycloak
go to http://loclahost:8080/auth

Credential: 
* login : admin
* password:  Pa55w0rd

# Modify theme
Go into the realm settings, click on the 'Themes' tab and pick 'my-logo-example'

# Stop
```
CTRL+C
docker-compose down
docker volume rm keycloak_postgres_data
```

