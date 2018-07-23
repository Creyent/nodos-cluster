# Payara-Dockerized

## Payara cluster node

Docker-compose file for a cluster SSH node.
Volumes persist all the files related to the node.

For use with the [payara-cluster](https://github.com/Creyent/payara-cluster) setup.
I decided to separate just the node for simplify the use on remote servers and scalability.

## Docker composer specifications

- Ubuntu 18.04 base
- OpenSSH
- OpenJDK 8

Note: This configuration was made on Windows 10. On Linux the shared folders are not setted before because it works out of the box.
The usual IP used for docker is (192.168.99.100), if differs please replace for your actual setup.

## Requirements

- Docker
- VirtualBox (usually installed with docker)
- GIT (just for clone this repo)

## Installation

- Go into any terminal and clone or fork the project.
- Browse into cloned folder:
    ```bash
    $ cd nodos-cluster
    ```
- Create a `.env` from the `.env.dist` file. Configure it according to your needs.
    ```bash
    cp .env.dist .env
    ```
- Build the required images typing in the docker terminal:
    ```bash
    $ docker-compose build
    ```

## Use

- Once cloned, go into folder:
    ```bash
    $ cd nodos-cluster
    ```
- Create and run the containers typing in the docker terminal:
    ```bash
    $ docker-compose up -d
    ```

## Comments

Any comment feel free to mail me: creyent [at] gmail [dot] com

## Contributing

Thanks for contributing!
If you find errors/typos/anything/... please send me a Pull Request, mail me or open an issue.