# JobQuest - React Job Board

JobQuest is a modern and responsive web application for browsing, adding, and managing job listings. Built with React and Vite, it offers a fast and interactive user experience. The application uses Tailwind CSS for styling and is powered by a `json-server` mock backend, making it a perfect project for demonstrating full CRUD (Create, Read, Update, Delete) functionality in a React environment.

## Features

-   **Browse Jobs**: View all available job listings on a clean, responsive interface.
-   **View Job Details**: Click on any job to see a detailed description, salary, and company information.
-   **Add a Job**: Easily add new job listings through a dedicated form with clear input fields.
-   **Edit a Job**: Update the details of any existing job listing.
-   **Delete a Job**: Remove job listings with a simple confirmation prompt.
-   **Responsive Design**: The UI is fully responsive and looks great on desktops, tablets, and mobile devices.
-   **User Notifications**: Integrated `react-toastify` to provide clear feedback for actions like adding, updating, and deleting jobs.
-   **404 Page**: A custom "Not Found" page for handling invalid routes.

## Tech Stack

-   **Frontend**:
    -   [React](https://react.dev/)
    -   [React Router](https://reactrouter.com/) for client-side routing
    -   [Vite](https://vitejs.dev/) as the build tool and development server
    -   [Tailwind CSS](https://tailwindcss.com/) for utility-first styling
-   **Backend**:
    -   [JSON Server](https://github.com/typicode/json-server) for a mock REST API

## Prerequisites

Before you begin, ensure you have the following installed on your system:
-   [Node.js](https://nodejs.org/) (v18 or later recommended)
-   [npm](https://www.npmjs.com/) (Node Package Manager)

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### 1. Clone the Repository

```bash
git clone [https://github.com/your-username/jobquest.git](https://github.com/your-username/jobquest.git)
cd jobquest
```

### 2. Install Dependencies

Install the necessary npm packages for both the client and the server.

```bash
npm install
```

### 3. Set Up the Backend Data

Create a file named `jobs.json` inside the `src/` directory. This file will act as your database. Paste the following sample structure into it:

```json
{
  "jobs": [
    {
      "id": "1",
      "title": "Senior React Developer",
      "type": "Full-Time",
      "description": "We are seeking a talented Front-End Developer to join our team in Boston, MA. The ideal candidate will have strong skills in HTML, CSS, and JavaScript, with experience working with React.",
      "location": "Boston, MA",
      "salary": "₹12L - 15L",
      "company": {
        "name": "Tech Solutions Inc.",
        "description": "Tech Solutions Inc. is a leading provider of innovative software solutions.",
        "contactEmail": "contact@techsolutions.com",
        "contactPhone": "555-555-5555"
      }
    },
    {
      "id": "2",
      "title": "Node.js Backend Developer",
      "type": "Remote",
      "description": "Join our team as a Backend Developer specializing in Node.js. You will be responsible for building and maintaining our server-side logic and APIs.",
      "location": "Remote",
      "salary": "₹15L - 17.5L",
      "company": {
        "name": "Web Services Co.",
        "description": "Web Services Co. provides scalable cloud solutions for businesses of all sizes.",
        "contactEmail": "careers@webservices.com",
        "contactPhone": "555-555-5556"
      }
    }
  ]
}
```

### 4. Run the Application

You will need to run two commands in separate terminal windows: one for the backend `json-server` and one for the frontend Vite development server.

**Terminal 1: Start the Backend Server**
```bash
npm run server
```
This will start the JSON server on `http://localhost:8000`.

**Terminal 2: Start the Frontend Server**
```bash
npm run dev
```
This will start the Vite development server, and you can now view the application in your browser, usually at `http://localhost:5173`.

## Available Scripts

In the project directory, you can run:

-   `npm run dev`: Runs the app in development mode with hot-reloading.
-   `npm run server`: Starts the JSON Server mock API.
-   `npm run build`: Builds the app for production to the `dist` folder.
-   `npm run preview`: Serves the production build locally to preview it.