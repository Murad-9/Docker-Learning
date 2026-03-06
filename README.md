# Docker Learning
This is a small learning project where I explored running a Flask application inside a Docker container. The goal was to understand Dockerfiles, container builds, and Docker Compose, and to get comfortable with the workflow of building and running containerised apps.

What’s in this project

app.py – a simple Flask app with three routes:

/ – shows a visit counter

/about - about page

/health – health check endpoint

requirements.txt – lists Python dependencies: Flask and the Redis client

Dockerfile – defines the container image for the Flask app

docker-compose.yml – sets up the Flask app and Redis container to run together




What I learned

How to write a Dockerfile for a Python Flask app

The difference between docker build/docker run and docker-compose build/docker-compose up

Using Redis as a separate service and connecting it to Flask through the Python Redis client

Debugging common mistakes, such as:

Using the wrong import (from redis import redis vs from redis import Redis)

Port mismatches between the container and the host

Forgetting to rebuild the container after changing code or dependencies



Notes

This project was mainly for practising Docker workflows and troubleshooting small issues. It helped me solidify my understanding of:

Multi-container apps

Python Flask basics

Docker networking and ports

Even small mistakes — like a typo in app.py or using docker run instead of docker-compose — were valuable learning experiences that helped me understand how everything connects in practice.
