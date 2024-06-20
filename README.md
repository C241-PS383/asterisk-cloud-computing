# Backend Server Documentation

## Overview

This document provides a comprehensive overview of the backend server for our project, detailing the technologies and services used, as well as the deployment and development environment setup.

## Technologies and Frameworks

### Node.js
- **Programming Language:** The backend server is developed using Node 20.
- **Framework:** We use Express.js as the framework for building the server-side application.

### Google Cloud Services
- **Google Cloud Run:** Our backend server is continuously deployed to Google Cloud Run, for scalability, and cost-effecient deployment.
- **Google Cloud Functions:** We utilize Google Cloud Functions for Python to handle data preprocessing required by our model, which runs on TensorFlow.js.
- **Google Cloud Firestore:** Firestore serves as our primary database for handling login/registration and data storage.
- **Google Cloud Storage:** We store Docker images in Google Cloud Storage Buckets for efficient containerization and deployment.

### APIs and Libraries
- **TensorFlow.js:** Used for running machine learning models on the server.
- **Google Maps API:** Used to fetch and manage restaurant information.

## Development Environment

### WSL2 (Windows Subsystem for Linux)
- **Purpose:** We use WSL2 to develop the backend in a Linux virtual machine for better compatibility and ease of use with various tools and libraries required for development.

### Docker
- **Containerization:** We use Docker for containerizing our backend server, ensuring consistent environments across development, testing, and production.

### Additional Tools
- **Gcloud SDK:** Used for command-line interaction with Google Cloud services.
- **Visual Studio Code (VSCode):** The primary IDE for development.
- **Postman:** Utilized for testing the backend APIs.

## Detailed Components

### Node.js with Express
- **Setup:** Initialize a Node.js project, install all the required dependencies in specified in the package.json file, and define routes for handling API requests.

### Google Cloud SDK
- **Setup:** Install the Google Cloud SDK, login through the Google Cloud SDK, and set the project in Google Cloud SDK.

### Google Cloud Run
- **Deployment:** Create a Dockerfile, build the Docker image using Docker command line, test the container locally, push it to Google Container Registry, and deploy it to Google Cloud Run.

### Google Cloud Functions
- **Setup:** Create a Python function for data preprocessing and deploy it to Google Cloud Functions.

### Google Cloud Firestore
- **Usage:** Initialize Firestore in the Node.js application for handling login/registration and storing application data.

### Google Maps API
- **Fetching Restaurant Information:** Setup a project with billing account, and enable the Google Maps API to retrieve and process data about restaurants.

### Development Using WSL2
- **Setup:** Install WSL2 on Windows and set up a Linux distribution (Ubuntu distro). Install Node.js, npm, Docker, and other necessary tools within the WSL2 environment.

### Docker for Containerization
- **Creating Docker Images:** Write a Dockerfile to define the container image for the Node.js application. Build and store images in Google Cloud Storage.
