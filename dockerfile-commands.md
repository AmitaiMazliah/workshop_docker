# Essential Dockerfile Commands

1. FROM: Choosing the base image

    The FROM command specifies the base image for your Docker image. It's the starting point for your image and typically represents the operating system and runtime environment.

    `FROM nginx:stable`

2. LABEL: Adding metadata

    The LABEL command adds metadata to the image, such as version information, author, and description. It's helpful for documentation and organization.

    `LABEL maintainer="Your Name <your.name@example.com>"`

3. ENV: Setting environment variables

    With the ENV command, we establish environment variables within the container. These variables become accessible to the applications running within the container.

    `ENV DB_HOST=localhost DB_PORT=5432`

4. RUN: Executing Commands

    The RUN command executes shell commands within the container during the image build. It's often used to install software packages and configure the environment.

    `RUN apt-get update && apt-get install -y nginx`

5. COPY and ADD: Adding files and directories

    The COPY and ADD commands copy files and directories from the host into the container. COPY is used for straightforward file copying, while ADD can also handle URL downloads and extraction of compressed archives.

    `COPY ./app /app`

6. WORKDIR: Setting the working directory

    The WORKDIR command designates the working directory within the container. Subsequent commands execute within the context of this directory.

    `WORKDIR /app`

7. EXPOSE: Exposing ports

    The EXPOSE command informs Docker that the container will listen on specified ports at runtime.

    `EXPOSE 80`

8. CMD : Defining the default command

    The CMD command specifies the default command to run when the container starts. It provides the default behavior for the container

    `CMD ["nginx", "-g", "daemon off;"]`

9. ENTRYPOINT: Run a command

    It configures the container to run as an executable, providing a way to set a default command and accept additional parameters.

    `ENTRYPOINT ["executable", "param1", "param2"]`

10. ARG: Build time variable

    Define build-time variables that can be passed to the Docker build process.

    `ARG APP_VERSION=1.0`

11. USER: Specific the container's user

    Define a user inside the container, the default is the ROOT user.

    `USER appuser`