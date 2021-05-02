# Kong / Konga / Keycloak: securing API through OIDC

## Credits
[Securing APIs with Kong and Keycloak - Part 1](https://www.jerney.io/secure-apis-kong-keycloak-1/) by Joshua A Erney

## Requirements

- [**docker**](https://docs.docker.com/install/)
- [**docker-compose**](https://docs.docker.com/compose/overview/)
- Patience
- :coffee:

## Start

```
    docker-compose up -d
```
### Notes with the kong migrations

- When you are starting a new installation, execute the service named `kong-migrations`.

```
docker-compose run --rm kong-migrations
```

- When you are upgrading from an existing installation, execute the service named `kong-migrations-up`

```
docker-compose run --rm kong-migrations-up
```

- When you want to swipe the board clean, prune...

```
docker system prune
docker volume prune
```