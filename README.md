# MovieApp

## Overview

MovieApp is a web application that allows users to search for movies, add them to their favourites, and manage their favourite movies. It includes user authentication for login and registration.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Project](#running-the-project)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- [Node.js](https://nodejs.org/) (version 14.x or later)
- [npm](https://www.npmjs.com/get-npm) (version 6.x or later)
- [Git](https://git-scm.com/)

## Installation

1. **Clone the repository:**
    ```bash
    git clone git@github.com:your-username/your-repository.git
    cd your-repository
    ```

2. **Install dependencies for both frontend and backend:**

    **Frontend:**
    ```bash
    cd frontend
    npm install
    ```

    **Backend:**
    ```bash
    cd ../backend
    npm install
    ```

## Running the Project

1. **Start the backend server:**
    ```bash
    cd backend
    npm start
    ```

    The backend server will run on `http://localhost:5000`.

2. **Start the frontend development server:**
    ```bash
    cd ../frontend
    npm start
    ```

    The frontend development server will run on `http://localhost:3000`.

## Project Structure

Here is the basic structure of the project:

your-repository/
├── backend/
│ ├── server.js
│ ├── routes/
│ ├── models/
│ └── package.json
├── frontend/
│ ├── src/
│ │ ├── components/
│ │ ├── App.js
│ │ ├── index.js
│ │ ├── App.css
│ │ ├── auth.css
│ │ └── setupProxy.js
│ ├── public/
│ └── package.json
├── .gitignore
└── README.md

## Technologies Used

- **Frontend:**
  - React.js
  - Bootstrap
  - Axios

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB (optional, if you plan to use it for storing user data)

- **Authentication:**
  - JSON Web Tokens (JWT)

## Components Overview

### Frontend Components

- **AddFavourite.js:** Displays the "Add to Favourites" button.
- **LandingPage.js:** Landing page component with login and register options.
- **Login.js:** Handles user login.
- **Register.js:** Handles user registration.
- **MovieList.js:** Displays a list of movies.
- **MovieListHeading.js:** Displays headings for movie lists.
- **RemoveFavourite.js:** Displays the "Remove from Favourites" button.
- **SearchBox.js:** Search input for finding movies.

### Backend

The backend handles user authentication and serves as an API for the frontend. It is set up with the following structure:

- **server.js:** Main server file.
- **routes/**: Directory containing route files for handling API requests.
- **models/**: Directory containing Mongoose models (if using MongoDB).

## Setting Up Environment Variables

Create a `.env` file in the `backend` directory and add the following variables:
PORT
JWT_SECRET
MONGODB(If you are using it)

## Notes

- Ensure you replace `your-username` and `your-repository` with your actual GitHub username and repository name.
- If you encounter issues with permissions when cloning the repository, make sure your SSH keys are correctly configured.
