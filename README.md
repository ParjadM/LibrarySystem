# LibrarySystem

LibrarySystem is a Node.js and Express application for browsing a gallery of library-style images, logging in with local credentials, and placing orders for selected items.

## Features

- User login with credentials stored in `user.json`
- Gallery view backed by MongoDB
- Order flow for selecting and purchasing an image
- Session-based authentication
- Handlebars views for server-rendered pages

## Tech Stack

- Node.js
- Express
- express-handlebars
- client-sessions
- MongoDB

## Prerequisites

- Node.js 18 or newer
- npm
- A MongoDB Atlas or local MongoDB instance

## Installation

1. Clone the repository.
2. Install dependencies:

```bash
npm install
```

## Configuration

The app connects to MongoDB from `server.js` and `order.js`. Before running the project, make sure the MongoDB connection string is valid for your environment.

The local login credentials are loaded from `user.json`.

## Run the App

Start the server with:

```bash
npm start
```

The app runs on port `3000`.

Open the application in your browser at:

```bash
http://localhost:3000
```

## Project Structure

- `server.js` main Express application and routes
- `order.js` order-related routes
- `user.json` local username and password data
- `package.json` project metadata and scripts

## Notes

- The app expects Handlebars views and public assets to be available in the project structure used by the server.
- If MongoDB is unavailable, the gallery and order pages will not function correctly.