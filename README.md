# Dockerized Nginx Reversed Proxy and ACME companion

## Building for development/local docker

There is an .env.example file.
Make your changes there and rename it to .env
The start the image.

    $ docker compose up -d

Then stop the container:

    $ docker compose down

Locally you have to create the shared network:

    $ docker create network kali-net

Add these to you .env and rebuild/restart the conainer:

    $ docker compose up -d --build --force-recreate

For further documentation see the official guide at https://beszel.dev/.

## Deployment

Deployment is done by Github actions.

