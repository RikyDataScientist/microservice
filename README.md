## 📦 Microservices Backend with Docker & Docker Compose

This repository contains an implementation of a microservices architecture using Docker and Docker Compose, developed as part of the Computer Architecture and Operating Systems course project.

The system is designed with a modular approach, where each service runs independently in its own container while remaining fully integrated through Docker’s internal networking.

---

## 🧩 System Architecture

The project consists of the following core services:
- API Gateway (Nginx)
Acts as the main entry point (single entry point) for all client requests and handles request routing to the appropriate backend services.
- Auth Service
An authentication service built with Node.js and MongoDB as its database.
Manages user accounts and authentication using JWT (JSON Web Token).
- Academic Service (Acad Service)
A backend service responsible for managing academic data using PostgreSQL.
Provides an API endpoint to calculate the Semester Grade Point Average (GPA/IPS) based on course grades and credit units (SKS).
- Separated Databases per Service
MongoDB → Auth Service
PostgreSQL → Academic Service

---

## ⚙️ Technologies Used

- Docker & Docker Compose
- Nginx (API Gateway)
- Node.js
- MongoDB
- PostgreSQL
- RESTful API (JSON responses)

---

## 🚀 Key Features

- Multi-container orchestration using Docker Compose
- Inter-service communication via Docker Network
- Centralized request routing with API Gateway
- Automatic GPA (IPS) calculation
- Data validation and backend error handling
- Data persistence using Docker Volumes

---

## 🧪 API Testing

API endpoints are tested using Thunder Client to ensure:

- All services run correctly
- Proper HTTP status codes are returned
- Consistent and well-structured JSON responses

---

## 🎯 Project Objectives

- Understand microservices architecture concepts
- Apply containerization in backend development
- Practice modern backend development patterns (API, database integration, error handling)
- Build an integrated and scalable distributed system

---