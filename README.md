    npx @vue/cli create vue-nginx-docker
    cd vue-nginx-docker
    touch Dockerfile
    echo "node_modules" > .dockerignore

After edit docker file by two stage,run

    docker build -t vue-nginx .
    docker run --rm -it -p 8080:80 vue-nginx

# vue-nginx-docker

## Project setup

```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
