# Let's (Do)cker

This is a workshop to learn Docker.

## Installation

Throughout the workshop, we will use dev-containers to minimize the setup time and ensure alignment between participants.
You may choose to avoid dev-containers and set up your local environment. 
However, I will have limited capacity to help you with the setup during the workshop.
If you do choose to set up your local environment, please follow the manual instructions in the next section below.

### Dev Containers (Recommended)
1. Docker
    
    a. Install Docker Desktop: https://www.docker.com/products/docker-desktop
    
    b. Validate the installation by running the following command in your terminal:
    ```bash
    docker --version
    ```

2. Visual Studio Code

    - Install Visual Studio Code: https://code.visualstudio.com/

    - Windows Only step
    
        Add this to your user-settings json file: `"dev.containers.forwardWSLServices": false`
    
        Or, using the GUI: `ctrl+shift+p` --> `Preferences: Open User Settings` --> enter this in the search box: `"dev.containers.forwardWSLServices"` and uncheck it. restart VS Code afterwards.

        Consider turning this back to `true` after the workshop, if required.

    - Install the Dev-Containers extension: https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers

    - Clone this repository to your local machine.

    - In Visual Studio Code, open the command pallette (Cmd/Ctrl+Shift+P) and run the command dev "Dev Containers: Open Folder in Container"

    - In the small pop-up, click the `(show logs)` link to enjoy the show. 😄

    - Wait until the container is built and the workspace is opened in the container.

3. That's it! (The magic of dev-containers 😉)