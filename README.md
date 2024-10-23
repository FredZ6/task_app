Task Management System

A task management system built with Spring Boot, React, PostgreSQL, and Docker. This project allows users to manage their tasks with features like creating, updating, and deleting tasks. The project includes a backend API, a frontend web application, and is containerized using Docker.

Table of Contents

	•	Features
	•	Technologies Used
	•	Installation
	•	Usage
	•	API Endpoints
	•	Contributing
	•	License

Features

	•	User authentication (Basic Auth using Spring Security).
	•	Create, read, update, and delete (CRUD) tasks.
	•	Manage task due dates and descriptions.
	•	Dockerized environment for easy deployment.
	•	PostgreSQL as the database.
	•	Frontend built using React.

Technologies Used

	•	Backend: Spring Boot (Java)
	•	Frontend: React.js
	•	Database: PostgreSQL
	•	Containerization: Docker
	•	Build tool: Maven
	•	CSS Framework: Material UI

Installation

Prerequisites

Make sure you have the following installed:

	•	Docker
	•	Git

Steps

	1.	Clone the repository:

git clone https://github.com/FredZ6/task_app.git
cd task-management-system


	2.	Run the application using Docker Compose:
Make sure Docker is running and then use the following command to start the project:

docker-compose up --build

This will start the backend, frontend, and database services.

	3.	Access the application:
	•	Frontend: Open your browser and go to http://localhost:3000
	•	Backend API: The backend is running at http://localhost:8080

Usage

Default Login

By default, the application creates an in-memory user during initialization. You can use the following credentials for initial access:

	•	Username: user
	•	Password: The password will be generated during startup and printed in the backend logs. Look for a line like:

Using generated security password: [generated-password]



Managing Tasks

Once logged in, you can:

	•	Create a new task by providing a title and due date.
	•	View all your tasks on the dashboard.
	•	Edit or delete tasks as needed.

API Endpoints

Method	Endpoint	Description
POST	/api/tasks/create	Create a new task
GET	/api/tasks	Get a list of all tasks
GET	/api/tasks/{id}	Get a task by its ID
PUT	/api/tasks/{id}	Update a task by its ID
DELETE	/api/tasks/{id}	Delete a task by its ID

Contributing

If you’d like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

Steps to Contribute

	1.	Fork the repository.
	2.	Create your feature branch: git checkout -b feature/my-feature.
	3.	Commit your changes: git commit -m 'Add some feature'.
	4.	Push to the branch: git push origin feature/my-feature.
	5.	Open a pull request.

License

This project is licensed under the MIT License - see the LICENSE file for details.
