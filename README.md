# Book System REST API

This is a simple Node.js Express REST API to manage a list of books (in-memory, no database).

## Features
- **GET /books**: Get all books
- **POST /books**: Add a new book (provide `title` and `author` in JSON body)
- **PUT /books/:id**: Update a book by ID (provide `title` and/or `author` in JSON body)
- **DELETE /books/:id**: Delete a book by ID

## How to Run
1. Install dependencies:
   ```sh
   npm install
   ```
2. Start the server:
   ```sh
   node index.js
   ```
3. The server runs on [http://localhost:3000](http://localhost:3000)

## Testing
- Use [Postman](https://www.postman.com/) or similar tool to test the endpoints.
- Example book object:
  ```json
  {
    "title": "Book Title",
    "author": "Author Name"
  }
  ```

## Notes
- All data is stored in memory and will be lost when the server restarts.
