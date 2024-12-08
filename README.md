# Chennells Farm Website

## This guide outlines the steps to set up, build, and run this application using virtual environments (venv) and Docker containers.

### Table of contents:
1. Prerequisites
2. Cloning the repository
3. Creating a virtual environment
4. Activating the virtual environment
5. Installing dependencies
6. Build the docker image
7. Run the container

### 1. Prerequisites

**Git**
https://git-scm.com/downloads

**Python**
https://www.python.org/downloads/ (version specified in requirements.txt)

**Docker Desktop**
https://www.docker.com/ (for Docker container build and execution)

### 2. Clone the repository

> **Bash**
> git clone https://github.com/keedenf/chennells-website.git

Navigate to the project directory:
> **Bash**
> cd chennells-website

### 3.Create a virtual environment

> **Bash**
> python -m venv venv

### 4.Activate the virtual environment

_**Linux/macOS:**_
> **zsh**
> source venv/bin/activate

_**Windows:**_
> **Bash**
> venv\Scripts\activate

### 5.Install dependencies

> **Bash**
> pip install -r requirements.txt

## Building and Running with Docker

### 6.Build the Docker image

> **Bash**
> docker build -t chennells-website .

### 7.Run the container

> **Bash**
> docker run --publish 8000:8000 chennells website
_This command maps the container port (usually unspecified) to your host machine port 8000. You can access the application by visiting http://localhost:8000 in your web browser._
