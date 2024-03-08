# Docker rails
I have test docker and rails with this project in rails 7.1. I have used the following commands to build and run the project.

```bash
docker compose build
docker compose up
```

Generating and migrating something with rails
```bash
docker compose run --rm web bundle exec rails g scaffold comment
docker compose run --rm web bundle exec rails db:migrate
```

Going to the console
```bash
docker compose run --rm web bundle exec rails c
```

Opening container bash
```bash
docker exec -it docker-rails-mysql-1 bash # run this after running docker compose up
```
