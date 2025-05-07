# PhilosophicalDialogue

## Overview

This infrastructure has three containers: `jupyter`, `ollama-a`, `ollama-b`. 
- The `jupyter` container will launch a Jupyter server that is accessible through the 
host machine's browser at port 18888

## Setup Docker containers

- First, clone the repository

~~~bash
git config --global core.autocrlf false
git clone https://github.com/SmartGeese/PhilosophicalDialogue/
~~~

- Next, cd into the cloned repo and run the followings. 

~~~bash
cd PhilosophicalDialogue
docker compose build --no-cache base
docker compose build --no-cache jupyter
~~~

## Launch containers

- First, launch the `jupyter` container

~~~bash
docker compose up -d jupyter
~~~

- Next, launch the `ollama-` containers
~~~bash
docker compose up -d ollama-a
docker compose up -d ollama-b
~~~
