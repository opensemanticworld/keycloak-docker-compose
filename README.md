# keycloak-docker-compose

## Deploy

### Base
```bash
git clone https://github.com/OpenSemanticWorld/keycloak-docker-compose
cd keycloak-docker-compose
cp .env.example .env
docker compose up
```
## Overrides

e. g. to use caddy as reverse proxy (see [caddy-docker-proxy](https://github.com/OpenSemanticWorld/caddy-docker-proxy))
```bash
cp docker-compose.caddy.example.override.yml docker-compose.override.yml
docker compose up
```

## Settings
.env:

| Key        | Description           | Example | Change |
| ------------- |:-------------:|:-----:|:-----:|
| KEYCLOAK_SERVER | Domain for the web UI and API | https://keycloak.example.com | Required |
| KEYCLOAK_ADMIN | Admin user name | admin | Recommended |
| KEYCLOAK_ADMIN_PASSWORD | admin password | change_me | Recommended |

## Further readings

- https://www.keycloak.org/server/all-config
