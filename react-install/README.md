Before using this Dockerfile create the react app with this command:

    docker exec -itu 1000:1000 react npx create-react-app /usr/src/app
    
Then, comment the specified lines inside the docker-compose.yml.
