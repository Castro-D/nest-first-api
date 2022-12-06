<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Dev environment

1.Clone repo

2.Run

```
npm install
```

3.Install nest cli

```
npm install -g @nestjs/cli
```

4.Init database

```
docker-compose up -d
```

5.Clone file `.env.template` and rename to `.env`

6.Change env variables.

7.Run app in dev mode:

`npm run start:dev`

8.Run seed:

`http://localhost:3000/api/v2/seed`

## Stack

- MongoDB
- Nestjs

# Production build

1.Create file `.env.prod` and fill variables

2.To build Image:

`docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build`

To run image:

`docker-compose -f docker-compose.prod.yaml --env-file .env.prod up`
