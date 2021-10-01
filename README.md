# Blog API

[![GitHub Licence](https://img.shields.io/github/license/mondesirm/blog)](https://gitlab.com/mondesirm/blog/-/blob/main/LICENCE)
[![Gitlab pipeline status](https://gitlab.com/mondesirm/blog/badges/main/pipeline.svg)](https://gitlab.com/mondesirm/blog/-/pipelines)
[![Gitlab code coverage](https://img.shields.io/gitlab/coverage/mondesirm/blog/main)](https://gitlab.com/mondesirm/blog/-/pipelines)

## Description
Ce projet utilise une base de données stockant les méta-données de films (nom et type) et une API qui retourne ces données sur la page d'accueil sous en format JSON.

## Technologies requises
- Docker ^20.10
- PHP ^8.0

## Installation
Avant de commencer, il est nécessaire d'installer les dépendances nécessaires au projet.
Dans la racine, tapez les commandes suivantes une par une :

```
docker compose up -d --build
docker compose exec php composer install
docker compose exec php php artisan migrate
docker compose exec php php artisan db:seed
docker compose exec php vendor/bin/phpunit 
```

La première commande lance les services

## Support
Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.

## Contributing
Si vous trouvez des bugs, vous pouvez nous aider à améliorer le projet en faisant une pull request (bugs seulement).

## Authors and acknowledgment
- [@mondesirm](https://gitlab.com/mondesirm)
- [@Arizona-dev](https://gitlab.com/Arizona-dev)
- [@Ampersander](https://gitlab.com/Ampersander)

## License
Voir [LICENCE](https://gitlab.com/mondesirm/blog/-/blob/main/LICENCE).