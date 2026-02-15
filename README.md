# Microservicios - API Gateway

API Gateway construido con .NET 8 y YARP (Yet Another Reverse Proxy) que proporciona enrutamiento, autenticaci√≥n y autorizaci√≥n centralizada para los microservicios.

## Tecnolog®™as

- **Autenticaci®Æn JWT** con Keycloak
- **Proxy reverso** con YARP
- **Contenedorizaci√≥n** con Docker

## Configuracion de Keycloak

### Keycloak

El API Gateway est√° configurado para autenticarse contra un servidor Keycloak externo:

- **URL**: `http://154.38.180.80:8080`
- **User admin**: admin
- **Password**: group3
- **Realm**: `group3realm`

##  Acceso al API Gateway

Una vez iniciado el contenedor, el API Gateway se publicar®¢ en: http://localhost:5666

### Endpoints de prueba:

- **Login**: `http://localhost:5666/api/login`
- **Users**: `http://localhost:5666/api/users` (requiere token)
- **Posts**: `http://localhost:5666/api/posts` (requiere token)

##  Autenticaci®Æn (Keycloak)

- **Grant Type**: `password`
- **Client ID**: `SuscripcionYContrato`
- **Client Secret**: `DGZvnuvbcpXh8Y8r8xjH87grc2z56r2H`
- **Username**: `tosmuer`
- **Password**: `77072732Contrato`