# Containerization Using Docker

## Definition

Containerization packages applications with dependencies into isolated environments called containers.
Docker is the most popular container platform.

---

# Components

Dockerfile  
Docker Image  
Docker Container

---

# Dockerfile

A script defining how to build a container.
Example:

FROM python:3.9
COPY app.py .
RUN pip install flask

---

# Docker Image

A snapshot containing application code and dependencies.
Images are used to create containers.

---

# Docker Container

A running instance of a Docker image.

---

# Benefits

Portability  
Consistency  
Isolation  
Scalability

---

# Typical Workflow

Code → Dockerfile → Image → Container
