# Docker for Sylius
This is a repository to run Sylius inside docker container using:

- PHP 8.0
- MariaDB
- Nginx

We recommand to use WSL instead Hyper-V on Windows or sell your gaming computer and take a laptop with a beautifull Linux OS. 
Note: This repo can run Symfony project too.
## Run WSL with CLI (only for Windows)
Start a simple CLI with Win + R and type `cmd`.
```
$ wsl -l -v
// Check version of WSL
$ wsl --set-default-version 2
// Change the version of WSL for version 2 (recommanded)
$ wsl --install -d Ubuntu
// Replace Ubuntu for a different Linux OS listed in this command: `wsl --list --online`
$ wsl -l -v
// Check if the distro has the good version. If it is not, run simply `wsl --set-version <distro> <version>` with: distro = distro name; version = version of WSL to use
```
## Installation of Docker
Download the Docker package(s) for your host system (https://docs.docker.com/get-docker/).
If you want Docker with WSL 2, take care about to thick "integration of WSL 2" during installation.
## Usage
Run the WSL (Windows) or regular CLI and navigate to your projects folder and run this commands:
```
$ mkdir src
// The `src` folder contains the project
$ git clone git@github.com:rayzen-io/DockerForSylius.git
$ cd DockerForSylius
$ docker-compose up
```
