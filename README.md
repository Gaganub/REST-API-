StudentAPI - ASP.NET Core Web API

📌 Overview:
StudentAPI is a simple RESTful API built using ASP.NET Core that demonstrates CRUD operations for managing student records. The API allows users to Create, Read, Update, and Delete (CRUD) student data.

🚀 Features:
RESTful API using ASP.NET Core

CRUD operations (Create, Read, Update, Delete) on student records

In-memory data storage (can be extended to a database)

CORS enabled for cross-origin requests

Swagger UI for easy testing

Structured API routes following REST principles

🛠️ Tech Stack

C#

ASP.NET Core 7/8

.NET 7/8 SDK

Swagger (API Documentation)

Postman / cURL (Testing)

Git & GitHub (Version Control)

📂 Project Structure

StudentAPI/
├── Controllers/
│   ├── StudentsController.cs  # Handles API requests
├── Models/
│   ├── Student.cs  # Defines Student model
├── Properties/
│   ├── launchSettings.json
├── Program.cs  # Main entry point
├── StudentAPI.csproj  # Project configuration
├── appsettings.json  # Configuration settings
├── .gitignore  # Ignored files for Git
└── README.md  # Project documentation

⚙️ Setup & Installation

1️⃣ Clone the Repository

git clone https://github.com/yourusername/StudentAPI.git
cd StudentAPI

2️⃣ Install .NET SDK (if not installed)

Download and install .NET SDK from here.

3️⃣ Run the API

dotnet run

This will start the server at:

http://localhost:5000

4️⃣ Test API Endpoints

You can use Swagger, Postman, or cURL to test the API:

🔹 Get All Students

curl -X GET http://localhost:5000/api/students

🔹 Add a Student

curl -X POST http://localhost:5000/api/students -H "Content-Type: application/json" -d '{"name": "Charlie", "course": "Cybersecurity"}'

🔹 Get a Single Student

curl -X GET http://localhost:5000/api/students/1

🔹 Update a Student

curl -X PUT http://localhost:5000/api/students/1 -H "Content-Type: application/json" -d '{"name": "Alice Updated", "course": "AI"}'

🔹 Delete a Student

curl -X DELETE http://localhost:5000/api/students/1

📌 API Endpoints

Method

Endpoint

Description

GET

/api/students

Get all students

GET

/api/students/{id}

Get student by ID

POST

/api/students

Create a new student

PUT

/api/students/{id}

Update an existing student

DELETE

/api/students/{id}

Delete a student

🛠️ Future Enhancements

✅ Connect to SQL Database using Entity Framework Core

✅ Implement JWT Authentication for security

✅ Deploy to Azure or AWS for production

✅ Add Logging & Exception Handling
