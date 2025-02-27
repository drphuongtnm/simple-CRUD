# Simple CRUD API using ExpressJS, TypeScript, MongoDB, and Nodemon

This is a simple CRUD (Create, Read, Update, Delete) API built using ExpressJS, TypeScript, MongoDB, and Nodemon. The API allows you to manage book data by providing endpoints to create, retrieve, update, and delete books.

## Prerequisites

Ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)
- [Postman](https://www.postman.com/) (for testing the API)

## Installation

1. Clone this repository:
   ```sh
   git clone <repository-url>
   ```
2. Navigate to the project folder:
   ```sh
   cd <project-folder>
   ```
3. Install dependencies:
   ```sh
   npm install
   ```

## Running the Project

To start the server, run:

```sh
npm run start
```

The server will start at `http://localhost:4000/`.

## API Endpoints

### Get all books

**GET** `http://localhost:4000/book`

- Retrieves all book records from the database.

### Get a specific book

**GET** `http://localhost:4000/book/:id`

- Retrieves a single book record by its ID.

### Create a new book

**POST** `http://localhost:4000/book`

- Creates a new book entry.
- **Body Example (JSON):**
  ```json
  {
    "title": "SGK",
    "author": "Viet Nam",
    "price": 100000
  }
  ```

### Update a book

**PUT** `http://localhost:4000/book/:id`

- Updates an existing book record.
- **Body Example (JSON):**
  ```json
  {
    "title": "SGK",
    "author": "Ho Chi Minh",
    "price": 100000
  }
  ```

### Delete a book

**DELETE** `http://localhost:4000/book/:id`

- Deletes a book record by its ID.

## Testing the API

Open **Postman** and use the above endpoints to send requests and test the CRUD functionality.

Happy coding! 🚀
