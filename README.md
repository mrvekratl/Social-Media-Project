# Social Media API (ASP.NET Core 8)

## 📌 Project Description
This project is a **RESTful Web API**-based social media platform designed to support modern social media features, including **post creation**, **commenting**, **liking**, and **following**. Built using **ASP.NET Core 8 and C#**, the platform is designed to be highly scalable, offering **real-time notifications with SignalR** and **caching with Redis** to improve performance. The API utilizes **JWT** and **OAuth** for secure user authentication, making it suitable for a wide range of real-world applications in social networking services, blogs, and more.

## 🚀 Technologies
- **Backend**: ASP.NET Core 8 Web API (for building scalable, high-performance web services)
- **Database**: Microsoft SQL Server, Entity Framework Core (for data management and ORM)
- **Authentication**: JWT & OAuth (Google, GitHub - ensures secure and flexible user authentication)
- **Real-Time Notifications**: SignalR (real-time bidirectional communication for notifications)
- **Caching**: Redis (for optimizing performance with in-memory data caching)
- **Testing**: xUnit (for ensuring code reliability and implementing unit tests)
- **Version Control**: Git & GitHub (for collaboration and version tracking)

## 📜 Features
- 🛡️ **User Authentication** (JWT and OAuth2 login)
- 📝 **Post Management** (CRUD operations)
- 💬 **Commenting and Like System**
- 🔔 **Real-Time Notifications** (Live updates with SignalR)
- ⚡ **Caching** (Redis for performance optimization)
- 🧪 **Unit Testing** (xUnit for code reliability)
- 🌍 **Docker & Deployment** (Azure App Services / AWS support)

## 📂 Project Structure

This project follows a **clean architecture** pattern, separating concerns into distinct layers for better maintainability and scalability. Here's a breakdown of the project structure:


| Folder                        | Description                                                   |
|-------------------------------|---------------------------------------------------------------|
| **SocialMedia.API**            | Web API Layer - Defines the API endpoints and handles client communication |
| **SocialMedia.Core**           | Business Logic and Models Layer - Contains core business logic and domain models |
| **SocialMedia.Infrastructure** | Data Access Layer - Responsible for interacting with the database using Entity Framework Core |
| **SocialMedia.Tests**          | Unit Tests - Contains tests to ensure API functionality and code reliability |
| **docker-compose.yml**         | Docker Configuration - For containerizing the application for deployment |
| **README.md**                  | Project Documentation - This file                           |


In this structure:

The API layer handles requests and responses.
The Core layer contains business logic and models that are independent of other layers.
The Infrastructure layer is responsible for database interactions and external services.
Tests are located in a separate directory for better separation of concerns.
This architecture makes it easier to maintain, scale, and test the project.


## 🛠️ Installation

Follow the steps below to set up the project locally:

### 1️⃣ Install Dependencies
Ensure that you have the following dependencies installed on your machine:

- **.NET SDK 8**: Download and install the SDK from [here](https://dotnet.microsoft.com/download/dotnet).
- **Microsoft SQL Server**: Install SQL Server from [here](https://www.microsoft.com/en-us/sql-server/sql-server-downloads).

### 2️⃣ Clone the Repository
Clone the repository to your local machine:

git clone https://github.com/your-username/social-media-api.git
cd social-media-api

### 3️⃣ Restore Dependencies
After cloning the repository, restore the required dependencies for the project using the .NET CLI:

dotnet restore

### 4️⃣ Initialize the Database
dotnet ef database update

### 5️⃣ Run the API
dotnet run

## 📌 API Endpoints

Here are the available API endpoints for interacting with the platform:

| Method | Endpoint                | Description                             |
|--------|-------------------------|-----------------------------------------|
| POST   | /api/auth/register       | Register a new user                     |
| POST   | /api/auth/login          | Login a user and retrieve JWT token     |
| GET    | /api/posts               | Retrieve a list of all posts            |
| POST   | /api/posts               | Create a new post                       |
| GET    | /api/posts/{id}          | Retrieve details of a specific post     |
| POST   | /api/posts/{id}/like     | Like a specific post                    |
| POST   | /api/posts/{id}/comment  | Post a comment on a specific post       |
| GET    | /api/notifications       | Retrieve notifications for the user     |


## 🔥 Contributing

Contributions to this project are welcome! To contribute:

1. **Fork the repository** to your own GitHub account.
2. **Clone your fork** to your local machine.
3. Create a new **branch** to work on your feature or fix.
4. **Implement the changes** and write tests to ensure functionality.
5. **Commit your changes** and push to your fork.
6. **Open a pull request** to the main repository for review.

Please make sure your changes pass existing unit tests before submitting your pull request.

For any questions or issues, feel free to **open an issue**. 🎯

---
🎉 **Contributing to this project will strengthen your backend development skills and demonstrate your ability to work on real-world applications!**


