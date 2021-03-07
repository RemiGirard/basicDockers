## Docker - simple servers

Basic configurations to run servers with Docker.

## Requirement
Docker Compose:
- Windows: https://docs.docker.com/docker-for-windows/install/
- Mac: https://docs.docker.com/docker-for-mac/install/
- Linux: https://docs.docker.com/engine/install + https://docs.docker.com/compose/install/


## Clone

`git clone https://github.com/RemiGirard/basicDockers.git`

## General use

Server | Command | Access | Comment
--- | --- | --- | ---
Ubuntu Server | `docker-compose up ubuntu` | Access the container with`docker-compose exec ubuntu bash` | 
Create react app | `docker-compose up create-react-app` | The new react app is created inside `react/app/` | Use `docker-compose up react` to start the app. It will then be available at https://localhost:3000
React | `docker-compose up react` | The app is available at https://localhost:3000. | **Requirement** : create a new react app with `docker-compose up create-react-app` **or** copy your existing react app in `react/app/` folder

## Configuration

### Create react app

By default, the app is created inside react/app folder. To change the name of the folder modify the `.env` file:

```
# create-react-app
CREATE_REACT_APP_FOLDER_NAME=app
```

### React

By default, your app has to be inside react/app folder. To change the name of the folder modify the `.env` file:

```
# react
REACT_APP_FOLDER_NAME=app
```