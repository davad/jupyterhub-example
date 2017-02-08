This example is based on the [JupyterHub demo](https://github.com/jupyterhub/jupyterhub-deploy-docker).

# Prerequisites

* Docker
* GNU Make (Apple Developer Tools on Mac, `sudo apt install
  build-essential` on Ubuntu)

# Getting Started

This example bundles a self-signed SSL certificate and information for a
GitHub client application that runs on `localhost`. To get started, run
the following commands:

```
make
docker-compose up
```

The JupyterHub server outputs the following when it's ready:
```
jupyterhub | [I 2017-02-08 06:11:32.361 JupyterHub app:1485] JupyterHub is now running at http://127.0.0.1:443/
```
You can kill the docker containers by pressing "Ctrl-C" in the terminal.

You'll be able to browse to https://localhost to interact with the
application. It will authenticate against your GitHub account.
