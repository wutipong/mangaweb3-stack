# Mangaweb3 Docker Compose Stack

## Getting Started

In order to get the stack running, two environment variables need to be set before running the stack. eg.

```env
DATA_PATH="./data"
HTTP_PORT=8080
```

This can be done by make a copy the file `dev.env` and rename it to `.env` before running the containers.

Alternatively you can specify the variable values via command line parameter directly.

Use `docker compose up -d` command to starts the containers.

## Running on Portainer

Running on Portainer needs the ability to mount volumes to project file, as we are injecting the `Caddyfile` configuration file to caddy. Unfortunately the *Enable relative path volumes* is only available on the business edition version of Portainer.

This flag needs to be set before deploying the stack, as it can't be set or reset afterward.

Make sure to set the environment variables before running the stack.
