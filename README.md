# node-on-docker
At first, Please overwrite this files.

## Prerequired

* Docker
* VSCode

## Build the Docker environment

* Please add this vscode plugin ([Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers))

* Overwrite Dockerfile
    - Update node version
    ```Dockerfile
        FROM node:XX
    ```

* Overwrite docker-compose.yml
    - Update service name
    ```yml
    services:
        please_write_the_service_name:
    ```
* Run Remote-container command (Shift + Ctrl + P)
    ```
    Remote-Containers: Add Development Container Configuration Files...
    From 'docker-compose.yml'

    > .devcontainer
    >   devcontainer.json
    >   docker-compose.yml
    ```

* Reopen Remote-container

* (On Remote) Run create-react-app
    ```
    npx create-react-app --template typescript service_name
    ```
