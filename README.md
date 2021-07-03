    npx @vue/cli create vue-nginx-docker
    cd vue-nginx-docker
    touch Dockerfile
    echo "node_modules" > .dockerignore

After edit docker file by two stage,run

    docker build -t vue-nginx .
    docker run --rm -it -p 8080:80 vue-nginx

