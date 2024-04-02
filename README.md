# SCHOOL MANAGEMENT SYSTEM
### Streamline school management, class organization, and add students and faculty. Seamlessly track attendance, assess performance, and provide feedback. Access records, view marks, and communicate effortlessly.

# About 
The School Management System is a web-based application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. It aims to streamline school management, class organization, and facilitate communication between students, teachers, and administrators.

# Features
**User Roles:** The system supports three user roles: Admin, Teacher, and Student. Each role has specific functionalities and access levels.

**Admin Dashboard:** Administrators can add new students and teachers, create classes and subjects, manage user accounts, and oversee system settings.

**Attendance Tracking:** Teachers can easily take attendance for their classes, mark students as present or absent, and generate attendance reports.

**Performance Assessment:** Teachers can assess students' performance by providing marks and feedback. Students can view their marks and track their progress over time.

**Data Visualization:** Students can visualize their performance data through interactive charts and tables, helping them understand their academic performance at a glance.

**Communication:** Users can communicate effortlessly through the system. Teachers can send messages to students and vice versa, promoting effective communication and collaboration.

# Technologies Used
- Frontend: React.js, Material UI, Redux
- Backend: Node.js, Express.js
- Database: MongoDB

# Installation

Open 2 terminals in separate windows/tabs.

Terminal 1: Setting Up Backend

cd backend

npm install

npm start
Create a file called .env in the backend folder. Inside it write this :

MONGO_URL = mongodb://127.0.0.1/school

Instead of this link write your database link.

Terminal 2: Setting Up Frontend

cd frontend

npm install

npm start

Now, navigate to localhost:3000 in your browser. The Backend API will be running at localhost:5000.

If this is not working then go to the src > redux > userRelated > userHandle.js

Write this after the import statements :

const REACT_APP_BASE_URL = "http://localhost:5000"

Now replace all process.env.REACT_APP_BASE_URL with REACT_APP_BASE_URL.

# Deployment

- Render - server side
- Netlify - client side

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.
