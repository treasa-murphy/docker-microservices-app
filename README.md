Docker Microservices Application

Overview

This project demonstrates a microservice-based architecture using Docker and Docker Compose. It 
integrates different technology stacks into a single, containerised system, showcasing real-world 
deployment practices.

The project was developed for COMP 30520: Cloud Computing at University College Dublin.

System Architecture
The system consists of four main components:

WebApp (Flask-based frontend) — Port 8090

API (FastAPI backend service) — Internal communication, not exposed externally

Database (PostgreSQL) — Internal service for data persistence

Adminer (Database management interface) — Port 8091

Services are deployed using Docker Compose, with dedicated frontend and backend networks ensuring 
proper isolation.

Technologies Used
Python 3.9 (Flask, FastAPI)

PostgreSQL

Adminer

Docker and Docker Compose

Project Structure
web_app/

app.py

student.html

requirements.txt

Dockerfile

api/

main.py

db_setup.py

requirements.txt

Dockerfile

.env — Environment variables for the database

docker-compose.yml — Defines all services

report.pdf — Report documenting setup steps and results

video.mp4 — Screen recording demonstrating the project

README.md — This file

How to Run
Clone this repository:

git clone git@github.com:treasa-murphy/docker-microservices-app.git
cd docker-microservices-app

Create a .env file in the project root:

POSTGRES_DB=student
POSTGRES_USER=postgres
POSTGRES_PASSWORD=password

Build and start the services:

docker compose up --build

Access the application:

WebApp: http://localhost:8090

Adminer: http://localhost:8091


Docker Compose orchestration

Course Info

Module: COMP30520 - Cloud Computing

Instructor: Dimitris Chatzopoulos

Teaching Assistant: John Byabazaire

Institution: University College Dublin (UCD)
