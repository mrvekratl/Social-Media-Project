Social Media API (ASP.NET Core 8)

📌 Project Description

This project is a RESTful Web API-based social media platform built using ASP.NET Core 8 and C#. Users can create posts, comment, like, and follow others. Additionally, it features real-time notifications with SignalR and caching with Redis.

🚀 Technologies

Backend: ASP.NET Core 8 Web API, C#

Database: Microsoft SQL Server, Entity Framework Core

Authentication: JWT & OAuth (Google, GitHub)

Real-Time Notifications: SignalR

Caching: Redis

Testing: xUnit

Version Control: Git & GitHub

📜 Features

🛡️ User Authentication (JWT and OAuth2 login)

📝 Post Management (CRUD operations)

💬 Commenting and Like System

🔔 Real-Time Notifications (Live updates with SignalR)

⚡ Caching (Redis for performance optimization)

🧪 Unit Testing (xUnit for code reliability)

🌍 Docker & Deployment (Azure App Services / AWS support)

📂 Project Structure

/SocialMediaAPI
│── SocialMedia.API          # Web API Layer
│── SocialMedia.Core         # Business Logic and Models Layer
│── SocialMedia.Infrastructure # Data Access Layer
│── SocialMedia.Tests        # Unit Tests
│── docker-compose.yml       # Docker Configuration
│── README.md                # Project Documentation

🛠️ Installation

1️⃣ Install Dependencies

Ensure that .NET SDK 8 and Microsoft SQL Server are installed.

2️⃣ Clone the Repository

git clone https://github.com/your-username/social-media-api.git
cd social-media-api

3️⃣ Restore Dependencies

dotnet restore

4️⃣ Initialize the Database

dotnet ef database update

5️⃣ Run the API

dotnet run

📌 API Endpoints

Method

Endpoint

Description

POST

/api/auth/register

User registration

POST

/api/auth/login

User login (JWT)

GET

/api/posts

Retrieve all posts

POST

/api/posts

Create a new post

GET

/api/posts/{id}

Retrieve a specific post

POST

/api/posts/{id}/like

Like a post

POST

/api/posts/{id}/comment

Comment on a post

GET

/api/notifications

Retrieve user notifications

🔥 Contributing

If you would like to contribute, feel free to open a pull request or create an issue. 🎯
