# Designway Javascript Task

# Movie Rental Store Application

This is a movie rental store application that allows users to browse and rent movies. It consists of a PostgreSQL database to store information about the movies, an Express.js API for server-side operations, and an Angular frontend for user interaction. The application also includes an admin panel for administrators to manage movies, customers, and rentals.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Frontend](#frontend)
- [Admin Panel](#admin-panel)
- [Authentication](#authentication)
- [Input Validation](#input-validation)
- [Logging and Error Handling](#logging-and-error-handling)

## Prerequisites

To run this application, you need to have the following installed:

- PostgreSQL database
- Node.js
- Angular CLI

## Installation

1. Clone the repository:

```
git clone <repository-url>
cd movie-rental-store
```

2. Set up the PostgreSQL database:

   - Create a new database in PostgreSQL.
   - Update the database connection details in the `config.js` file.

3. Install the backend dependencies and start the server:

```
cd backend
npm install
npm start
```

4. Install the frontend dependencies and start the Angular development server:

```
cd frontend
npm install
ng serve
```

## Usage

Once the server and frontend are running, you can access the application by visiting `http://localhost:4200` in your web browser.

## API Endpoints

The Express.js API provides the following endpoints:

- `POST /movies` - Add a new movie
- `PUT /movies/:id` - Update a movie
- `DELETE /movies/:id` - Delete a movie
- `POST /customers` - Add a new customer
- `PUT /customers/:id` - Update a customer
- `DELETE /customers/:id` - Delete a customer
- `GET /movies` - Browse movies by genre, title, and release year
- `POST /cart` - Add movies to the cart
- `POST /checkout` - Checkout the cart

For detailed request and response examples, refer to the API documentation.

## Frontend

The Angular frontend allows users to perform the following operations:

- Browse movies by genre, title, and release year
- Add movies to the cart
- View the contents of the cart
- Remove movies from the cart
- Checkout the cart

The frontend interacts with the backend API to fetch and update data.

## Admin Panel

The Angular admin panel allows administrators to perform the following operations:

- Add, edit, and delete movies
- Add, edit, and delete customers
- View a list of all rentals

Administrators can access the admin panel by visiting `http://localhost:4200/admin` in their web browser.

## Authentication

API endpoints and the admin panel are secured using JWT authentication. Users and administrators need to authenticate themselves by providing a valid JWT token in the request headers.

## Input Validation

Both the frontend and backend implement input validation to prevent invalid data from being submitted to the server. The application validates user input and provides appropriate error messages if validation fails.

## Logging and Error Handling

The application implements logging and error handling to track and handle runtime errors. Logs are generated for important events, and error messages are displayed to the users when something goes wrong.

---

This is just a sample README file that covers the basic structure of your project and the main components. You can

 customize it further to include additional information or instructions specific to your project.

Make sure to update the installation instructions and other sections with accurate information based on your project's setup.
