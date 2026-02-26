# Library Management System

A full-stack library management application built with React (frontend) and Express/MongoDB (backend). Features a clean black and white UI for managing books in a library.

## Project Structure

```
library-management/
├── backend/
│   ├── models/
│   │   └── Book.js
│   ├── package.json
│   └── server.js
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
├── .gitignore
└── ERRORS_AND_ISSUES.md
```

## Prerequisites

- Node.js (v14 or higher)
- MongoDB (running locally or remote connection)
- npm or yarn

## Installation and Setup

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Start the server:
```bash
npm start
```

The server will run on `http://localhost:5000`

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:3000`

## Features

- View all books in the library
- Add new books with title, author, and publication year
- Edit existing book information
- Delete books from the library
- Real-time UI updates

## API Endpoints

- `GET /api/books` - Retrieve all books
- `GET /api/books/:id` - Retrieve a specific book
- `POST /api/books` - Create a new book
- `PUT /api/books/:id` - Update a book
- `DELETE /api/books/:id` - Delete a book

## Data Model

Each book contains:
- `_id` - MongoDB ObjectId (auto-generated)
- `title` - Book title
- `author` - Author name
- `year` - Publication year
- `createdAt` - Creation timestamp (auto-generated)

## Intentional Issues

This application contains 5 intentional errors/issues in both the frontend and backend. These are documented in [ERRORS_AND_ISSUES.md](ERRORS_AND_ISSUES.md) for educational purposes.

## UI Design

The application uses a minimalist black and white design with:
- Black header with white text
- White content sections with black borders
- Grid layout for book cards
- Clear typography and spacing
- Responsive design

## Database

The application uses MongoDB to store book data. Ensure MongoDB is running before starting the backend server.
