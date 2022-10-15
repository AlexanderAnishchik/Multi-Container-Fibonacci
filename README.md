# multi-container-fibonacci
# Fibonacci calculation app (specially complicated with Redis and Postgres) built on docker's containers

![This is an image](https://upload.wikimedia.org/wikipedia/commons/3/35/Fibonacci2.jpg)

## Tech Stack
- React, Node.js
- Postgres, Redis
- Docker, docker-compose, Kubernetes
- Azure, AWS, Github

## Architecture
- client project - React UI simple application
- server project - Node.js API application works with Redis and Postgres
- worker - background project works with Redis

## Branches
- docker-compose contains configuration for local development and deployment of containers to AWS Elastic Beanstalk via Github Actions.
- master contains kubernetes cluster setup and Github Actions to deploy to Azure AWS

## How To Run
- To run docker-compose execute "docker-compose up -f docker-compose-dev.yml --build" in a solution directory. Open "localhost:80" URL in browser
- To run kubernetes execute "kubectl apply -f k8s" in a solution directory.
