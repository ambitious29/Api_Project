# Book Management API

## Introduction

The Book Management API is a RESTful API that allows you to manage books, authors, and publications. You can perform various operations such as adding new books, updating book details, retrieving book information by ISBN, and much more.

## Prerequisites

Before you can use the Book Management API, ensure you have the following prerequisites:

- Node.js and npm installed
- MongoDB set up and running
- Environment variables configured (see `.env.example`)
- Required Node.js packages (installed via `npm install`)

## Installation

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/ambitious29/Api_Project
Usage
To start the API server, run the following command:

bash
Copy code
npm start
The API server will be running on http://localhost:3000 by default. You can customize the port in the .env file.

Routes
The API provides the following routes:

GET /: Get all books.
GET /is/:isbn: Get a specific book by ISBN.
GET /c/:category: Get a specific book by category.
GET /author: Get all authors.
GET /author/book/:isbn: Get authors for a specific book.
GET /publications: Get all publications.
POST /book/new: Add a new book.
POST /author/new: Add a new author.
POST /publication/new: Add a new publication.
PUT /book/update/:isbn: Update a book by ISBN.
PUT /book/author/update/:isbn: Update or add an author to a book.
PUT /publication/update/book/:isbn: Update or add a publication to a book.
DELETE /book/delete/:isbn: Delete a book by ISBN.
DELETE /book/delete/author/:isbn/:authorId: Delete an author from a book and vice versa.
Please refer to the API code (index.js) for more details on each route and their request/response formats.

Contributing
Contributions to this project are welcome. You can open issues to report bugs or suggest enhancements. If you'd like to contribute code, please fork the repository and create a pull request.
