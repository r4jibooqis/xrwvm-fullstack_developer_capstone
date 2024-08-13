# Dealerships Website

## Overview

The "Dealerships Website" is a comprehensive web application designed to manage dealership information, car reviews, and sentiment analysis. This project utilizes modern web technologies, including Django, React, Node.js, Docker, and IBM Cloud Code Engine, to create a robust and scalable full-stack application.

## Project Structure

The project is divided into several key components:

1. **Django Application**: The main web application built using Django, providing the front-end and back-end functionality.
2. **React Frontend**: A React application integrated with Django for user management.
3. **Node.js Backend Service**: A service for managing dealership data and reviews, containerized using Docker.
4. **Sentiment Analyzer Service**: Deployed on IBM Cloud Code Engine for analyzing the sentiment of reviews.

## Architecture

![Architecture Diagram](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-CD0321EN-Coursera/labs/v2/m1/images/v2.capstone-dealership-architecture.png)

### Technologies Used

- **Django**: Python web framework for building the main application.
- **React**: JavaScript library for building user interfaces.
- **Node.js**: JavaScript runtime for the backend service.
- **Express**: Node.js framework for building RESTful APIs.
- **MongoDB**: NoSQL database used by the Node.js service.
- **Docker**: Containerization tool for deploying the Node.js service.
- **IBM Cloud Code Engine**: Platform for deploying the Sentiment Analyzer Service.
- **Kubernetes**: Container orchestration platform for deploying the application.

## Getting Started

### Prerequisites

- Python 3.8+
- Node.js 14+
- Docker
- IBM Cloud CLI (for deploying the Sentiment Analyzer Service)

### Setup Instructions

1. **Fork and Clone the Repository**

   Fork the repository from GitHub and clone it to your local environment.

   ```bash
   git clone https://github.com/your-username/dealerships-website.git
   ```

2. **Setup Django Application**

   Navigate to the Django application directory and install the required Python packages.

   ```bash
   cd django_app
   pip install -r requirements.txt
   ```

   Run the Django server locally.

   ```bash
   python manage.py runserver
   ```

3. **Setup React Frontend**

   Navigate to the React application directory and install the required Node.js packages.

   ```bash
   cd react_frontend
   npm install
   ```

   Start the React development server.

   ```bash
   npm start
   ```

4. **Setup Node.js Backend Service**

   Build and run the Node.js service using Docker.

   ```bash
   cd node_service
   docker build -t node-service .
   docker run -p 5000:5000 node-service
   ```

5. **Deploy Sentiment Analyzer Service**

   Deploy the Sentiment Analyzer Service on IBM Cloud Code Engine. Follow the instructions in the IBM Cloud documentation to deploy the service.

6. **Migrate Django Database**

   Apply the database migrations for Django.

   ```bash
   python manage.py migrate
   ```

### CI/CD Setup

1. **Continuous Integration and Delivery**

   Set up CI/CD pipelines for linting, testing, and deploying the application. This can be configured using tools like GitHub Actions or Jenkins.

2. **Deploy on Kubernetes**

   Deploy the application on Kubernetes using the provided Kubernetes configuration files.

   ```bash
   kubectl apply -f k8s/deployment.yaml
   kubectl apply -f k8s/service.yaml
   ```

## Project Breakdown

1. **Static Pages**: Created static pages to meet user stories.
2. **User Management**: Implemented user management with Django and React.
3. **Backend Services**: Developed Node.js service for managing dealerships and reviews, and deployed Sentiment Analyzer Service.
4. **Dynamic Pages**: Added dynamic pages using Django templates for displaying dealers and reviews.
5. **CI/CD**: Implemented CI/CD pipelines for code quality and deployment.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

