# Online-Library
ASP.NET Core MVC based Digital Library Management System with role-based authentication, book borrowing workflow, and pagination using SQL Server &amp; EF Core.
A full-stack Digital Library Management System built using ASP.NET Core MVC, Entity Framework Core, and SQL Server.
The application allows users to manage books, borrow and return them, and automatically calculates fines for overdue returns using real-world business logic.

Project Overview

This application is designed to simulate a real-world library management system. It enables administrators to manage book records and allows users to borrow and return books with automated fine calculation and secure role-based access control.

Features

Add, update, delete, and search books

Search books by title, author, or genre

Borrow and return functionality

Automatic fine calculation for overdue returns

Role-based authentication and authorization (Admin and User)

Pagination for handling large book lists

Server-side and client-side validations

Secure access control using ASP.NET Core Identity

Fine Calculation Logic

The system includes dynamic fine calculation functionality:

Calculates overdue days based on due date and return date

Applies configurable fine per day

Displays total fine at the time of return

Stores fine details in the database

Updates book availability after successful return

This ensures real-world usability and proper business logic implementation.

Architecture

The application follows a layered architecture:

Controller Layer – Handles HTTP requests and responses
Service Layer – Contains business logic such as fine calculation and validations
Repository Layer – Handles database operations
Database Layer – SQL Server

The project is implemented using:

MVC architectural pattern

Code-First approach with Entity Framework Core

Technology Stack

Backend

ASP.NET Core MVC

C#

ORM

Entity Framework Core

Database

Microsoft SQL Server

Frontend

HTML

CSS

JavaScript

Authentication

ASP.NET Core Identity

Role-Based Access Control

Database Design

Main entities include:

Users

Books

BorrowRecords

Roles

Relationships:

One User can have multiple Borrow Records

One Book can have multiple Borrow Records

Includes:

Foreign key constraints

Data annotations for validation

Optimized queries with indexing

Functional Modules

Book Management

Admin can add, edit, and delete books

View available and borrowed books

Search and filter functionality

Borrow and Return System

Users can borrow available books

Due date is automatically generated

Return updates book availability

Fine is calculated automatically for overdue returns

Pagination

Implemented pagination for book listings

Improves performance for large datasets

Reduces page load time

Setup Instructions

Clone the repository
git clone https://github.com/your-username/online-book-library.git

Update the connection string in appsettings.json

Run database migration
dotnet ef database update

Run the application
dotnet run

Future Enhancements

Email notifications for due date reminders

Book reservation feature

Online fine payment integration

Conversion to microservices architecture

Deployment to Azure

Learning Outcomes

Through this project, I gained practical experience in:

ASP.NET Core MVC architecture

Entity Framework Core Code-First approach

Role-based authentication and authorization

Business logic implementation for fine calculation

Database schema design and optimization

Pagination and performance improvement


Author
Saipriya Konda
Software Developer
