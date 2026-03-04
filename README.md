# MERN Task Manager

A full-stack task management web application built with the MERN stack (MongoDB, Express.js, React.js, and Node.js).

## Features

- **User Authentication**: Secure user registration and login functionality
- **Task Management**: Create, read, update, and delete tasks
- **Responsive UI**: Mobile-friendly interface built with React.js
- **Backend API**: RESTful API built with Node.js and Express.js
- **Database**: MongoDB for persistent data storage

## Project Structure

```
mern-task-manager/
├── server/                 # Node.js/Express backend
│   ├── models/            # MongoDB models
│   ├── routes/            # API routes
│   ├── controllers/        # Route controllers
│   ├── middleware/         # Custom middleware
│   └── server.js          # Main server file
├── client/                 # React.js frontend
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── pages/         # Page components
│   │   ├── App.js         # Main App component
│   │   └── index.js       # Entry point
│   └── package.json
├── package.json            # Root package.json
└── README.md
```

## Tech Stack

**Frontend**:
- React.js
- React Router
- Axios
- CSS/TailwindCSS

**Backend**:
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT (JSON Web Tokens)

## Installation

### Prerequisites
- Node.js and npm installed
- MongoDB installed and running

### Setup

1. Clone the repository:
```bash
git clone https://github.com/venkysk940-oss/mern-task-manager.git
cd mern-task-manager
```

2. Install backend dependencies:
```bash
cd server
npm install
```

3. Install frontend dependencies:
```bash
cd ../client
npm install
```

4. Configure environment variables in `server/.env`:
```
MONGODB_URI=mongodb://localhost:27017/task-manager
JWT_SECRET=your_jwt_secret
PORT=5000
```

5. Run the application:

**Backend** (from server directory):
```bash
npm start
```

**Frontend** (from client directory):
```bash
npm start
```

The application will be available at `http://localhost:3000`

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/logout` - Logout user

### Tasks
- `GET /api/tasks` - Get all tasks for logged-in user
- `POST /api/tasks` - Create a new task
- `PUT /api/tasks/:id` - Update a task
- `DELETE /api/tasks/:id` - Delete a task

## Usage

1. Register or login to your account
2. Create new tasks by clicking the "Add Task" button
3. Edit existing tasks by clicking the edit icon
4. Delete tasks by clicking the delete icon
5. Mark tasks as complete/incomplete

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - feel free to use this project in your own applications.

## Author

Venkatesh Sh (@venkysk940-oss)

## Support

For support, please open an issue in the repository.
