[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/NkrcaSS8)
# Microservicios - API Gateway

API Gateway construido con .NET 8 y YARP (Yet Another Reverse Proxy) que proporciona enrutamiento, autenticaciÃ³n y autorizaciÃ³n centralizada para los microservicios.

## Tecnolog¨ªas

- **Autenticaci¨®n JWT** con Keycloak
- **Proxy reverso** con YARP
- **ContenedorizaciÃ³n** con Docker

## Configuracion de Keycloak

### Keycloak

El API Gateway estÃ¡ configurado para autenticarse contra un servidor Keycloak externo:

- **URL**: `http://154.38.180.80:8080`
- **User admin**: admin
- **Password**: group3
- **Realm**: `group3realm`

##  Acceso al API Gateway

Una vez iniciado el contenedor, el API Gateway se publicar¨¢ en: http://localhost:5666

### Endpoints de prueba:

- **Login**: `http://localhost:5666/api/login`
- **Users**: `http://localhost:5666/api/users` (requiere token)
- **Posts**: `http://localhost:5666/api/posts` (requiere token)

##  Autenticaci¨®n (Keycloak)

- **Grant Type**: `password`
- **Client ID**: `SuscripcionYContrato`
- **Client Secret**: `DGZvnuvbcpXh8Y8r8xjH87grc2z56r2H`
- **Username**: `tosmuer`
- **Password**: `77072732Contrato`