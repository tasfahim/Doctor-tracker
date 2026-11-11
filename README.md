# Doctor Tracker



A full-stack doctor and patient management system designed to simplify healthcare record management through a centralized administrative dashboard.



Doctor Tracker provides an integrated platform for managing doctors, patients, and their associations, with authentication, dashboard analytics, search functionality, and user preferences.



## Project Structure



```text
Doctor-tracker/
|-- frontend/
|   |-- public/
|   |-- src/
|   |-- package.json
|   -- README.md
|
|-- backend/
|   |-- src/
|   |-- package.json
|   |-- .env.example
|   -- README.md
|
|-- .gitignore
-- README.md
```



## Features



- **Admin Authentication:** Secure administrative login and protected access.

- **Dashboard:** Overview of application statistics and visual analytics.

- **Doctor Management:** Create, view, update, and manage doctor records.

- **Patient Management:** Create, view, update, and manage patient records.

- **Doctor-Patient Association:** Manage relationships between doctors and patients.

- **Search and Filtering:** Find doctor and patient records efficiently.

- **Global Search:** Search across available application records.

- **Theme Preferences:** Light and dark theme support.

- **Language Preferences:** English and Bangla interface support.

- **API Integration:** Centralized communication between frontend and backend.



## Technology Stack



### Frontend

- Next.js

- React

- TypeScript

- Tailwind CSS

- Recharts

- Lucide React



### Backend

- Node.js

- Express.js

- TypeScript

- MongoDB

- Mongoose

- JSON Web Token (JWT)

- Zod



## Prerequisites



Before running the application, install:



- Node.js

- npm

- MongoDB database

- Git



## Installation and Setup



### 1. Clone the repository



```bash

git clone https://github.com/tasfahim/Doctor-tracker.git

cd Doctor-tracker

```



### 2. Configure the Backend



Navigate to the backend directory:



```bash

cd backend

npm install

```



Create a `.env` file in the backend directory using `.env.example` as a reference.



Configure the following environment variables:



| Variable | Description |

|---|---|

| `PORT` | Backend server port |

| `NODE_ENV` | Application environment |

| `CLIENT_URL` | Frontend origin allowed by CORS |

| `MONGODB_URI` | MongoDB connection string |

| `JWT_SECRET` | Secret used for JWT authentication |



Start the backend development server:



```bash

npm run dev

```



The backend runs locally at:



`http://localhost:5000`



Health check:



`http://localhost:5000/api/health`



### 3. Configure the Frontend



Open another terminal and navigate to the frontend directory:



```bash

cd frontend

npm install

```



Create a `.env.local` file in the frontend directory:



```env

NEXT_PUBLIC_API_URL=http://localhost:5000/api

```



Start the frontend development server:



```bash

npm run dev

```



Open the application:



`http://localhost:3000`



## Available Scripts



### Frontend



| Command | Description |

|---|---|

| `npm run dev` | Start development server |

| `npm run build` | Build production application |

| `npm run start` | Start production server |

| `npm run lint` | Run ESLint |



### Backend



| Command | Description |

|---|---|

| `npm run dev` | Start development server |

| `npm run build` | Compile TypeScript |

| `npm run start` | Start production server |



## Backend Architecture



The backend follows a modular structure:



- **Configuration:** Database connection and application configuration.

- **Models:** MongoDB data models for doctors, patients, and users.

- **Routes:** REST API endpoints and request handling.

- **Application:** Express middleware, security configuration, and error handling.

- **Server:** Database initialization and server startup.



## Security and Reliability



The application includes:



- JWT-based authentication.

- Password hashing.

- Helmet security middleware.

- CORS origin configuration.

- Rate limiting.

- Request validation.

- Centralized error handling.

- MongoDB connection management.

- Protection against deleting doctors with assigned patients.



## Repository Links



- **Main Repository:** https://github.com/tasfahim/Doctor-tracker

- **Frontend Repository:** https://github.com/tasfahim/doctor-tracker-frontend

- **Backend Repository:** https://github.com/tasfahim/doctor-tracker-backend



The frontend and backend repositories are maintained separately as independent project backups.



