# Backend Developer Intern Test

## Introduction

Welcome to the Backend Developer Intern Test. This test is designed to evaluate your proficiency in Node.js, JavaScript/TypeScript, and MongoDB by building a simple Blog Application with full CRUD (Create, Read, Update, Delete) functionalities.

## Requirements

You are required to develop a RESTful API for a Blog application using the following technologies:

- **Node.js**
- **JavaScript or TypeScript** (preferably TypeScript)
- **MongoDB**
- **Express.js** (or another framework of your choice)

## Task

You need to build a RESTful API that allows users to manage their blog posts. The API should include the following endpoints:

### Endpoints

#### 1. Create a Blog Post

- **Endpoint:**`<span>POST /blogs</span>`
- **Request Body:**
  ```
  {
    "title": "My First Blog Post",
    "content": "This is the content of my first blog post.",
    "author": "John Doe"
  }
  ```
- **Response:**
  ```
  {
    "id": "123456",
    "title": "My First Blog Post",
    "content": "This is the content of my first blog post.",
    "author": "John Doe",
    "createdAt": "2024-03-25T12:00:00Z"
  }
  ```

#### 2. Get All Blog Posts

- **Endpoint:**`<span>GET /blogs</span>`
- **Response:**
  ```
  [
    {
      "id": "123456",
      "title": "My First Blog Post",
      "content": "This is the content of my first blog post.",
      "author": "John Doe",
      "createdAt": "2024-03-25T12:00:00Z"
    }
  ]
  ```

#### 3. Get a Single Blog Post

- **Endpoint:**`<span>GET /blogs/:id</span>`
- **Response:**
  ```
  {
    "id": "123456",
    "title": "My First Blog Post",
    "content": "This is the content of my first blog post.",
    "author": "John Doe",
    "createdAt": "2024-03-25T12:00:00Z"
  }
  ```

#### 4. Update a Blog Post

- **Endpoint:**`<span>PUT /blogs/:id</span>`
- **Request Body:**
  ```
  {
    "title": "Updated Blog Post",
    "content": "This is the updated content of my blog post.",
    "author": "John Doe"
  }
  ```
- **Response:**
  ```
  {
    "id": "123456",
    "title": "Updated Blog Post",
    "content": "This is the updated content of my blog post.",
    "author": "John Doe",
    "updatedAt": "2024-03-25T14:00:00Z"
  }
  ```

#### 5. Delete a Blog Post

- **Endpoint:**`<span>DELETE /blogs/:id</span>`
- **Response:**
  ```
  {
    "message": "Blog post deleted successfully"
  }
  ```

## Technical Requirements

- Use **Express.js** for routing.
- Use **MongoDB** as the database, with Mongoose for schema modeling.
- The API should follow **RESTful principles**.
- Proper error handling and validation should be implemented.
- Use **TypeScript** if possible.

## Bonus Points

- Implement **JWT authentication** for securing the endpoints.
- Use **Docker** to containerize the application.
- Deploy the API to **Render, Vercel, Railway, or any cloud service**.

## Submission Guidelines

- Push your code to a **public GitHub repository**.
- Include a **README.md** explaining how to set up and run your project.
- Share the repository link once you're done.

Good luck! 🚀
