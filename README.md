# Preparation

## Install npm packages

```sh
docker-compose up -d
docker-compose exec node npm install
```

# Usage

## Build

webpack can detect file changes and rebuild after execute `npm start`.

```sh
docker-compose exec node npm start
```

when you want to production build, execute `npm run build`.
(this command don't detect file changes and rebuild.)

```sh
docker-compose exec node npm run build
```

## Load Chrome Extention

webpack will generate "dist" directory after build.
please load dist at [chrome://extensions/](chrome://extensions/).