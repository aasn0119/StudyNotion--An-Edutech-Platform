# StudyNotion Ed-Tech Platform (MERN App) 📚💻

StudyNotion is a fully functional ed-tech platform that enables users to create, consume, and rate educational content. The platform is built using the MERN stack, which includes ReactJS, NodeJS, MongoDB, and ExpressJS.

## Table of Contents

1. [Project Description](#project-description)
2. [System Architecture](#system-architecture)
   - [Architecture Diagram](#architecture-diagram)
3. [Front-end](#front-end)
   - [Pages for Students](#pages-for-students)
   - [Pages for Instructors](#pages-for-instructors)
   - [Pages for Admin (Future Scope)](#pages-for-admin-future-scope)
   - [Technologies Used](#technologies-used)
4. [Back-end](#back-end)
   - [Description](#description)
   - [Features and Functionalities](#features-and-functionalities)
   - [Technologies Used](#technologies-used-1)
   - [Data Models and Database Schema](#data-models-and-database-schema)
5. [API Design](#api-design)
   - [Sample API Endpoints](#sample-api-endpoints)
   - [Sample API Requests and Responses](#sample-api-requests-and-responses)
6. [Deployment](#deployment)
7. [Future Enhancements](#future-enhancements)
8. [Conclusion](#conclusion)

## Project Description

StudyNotion aims to provide:

- A seamless and interactive learning experience for students, making education more accessible and engaging.
- A platform for instructors to showcase their expertise and connect with learners across the globe.

![Front Page](/src/assets/Images/Picture1.jpg)

## System Architecture

The StudyNotion ed-tech platform consists of three main components: the front end, the back end, and the database. The platform follows a client-server architecture, with the front end serving as the client and the back end and database serving as the server.

![System Architecture](/src/assets/Images/Picture2.jpg)

- **Front-end**: Built using ReactJS, allows for the creation of dynamic and responsive user interfaces, critical for providing an engaging learning experience. Communicates with the back end using RESTful API calls.
- **Back-end**: Built using NodeJS and ExpressJS, providing APIs for the front end to consume. Handles user authentication, course creation, course consumption, and processes and stores course content and user data.
- **Database**: Built using MongoDB, a NoSQL database providing flexible and scalable data storage, useful for storing course content such as videos, images, and PDFs.

## Front-end 🎨

The front end is designed using Figma for a clean and minimal user interface. You can view the design [here](https://www.figma.com/file/Mikd0FjHKAofUlWQSi70nf/StudyNotion_shared).

### Pages for Students:

- **Homepage**: Brief introduction, links to the course list, and user details.
- **Course List**: List of all available courses with descriptions and ratings.
- **Wishlist**: Displays all courses a student has added to their wishlist.
- **Cart Checkout**: Allows course purchase completion.
- **Course Content**: Displays the course content including videos and other materials.
- **User Details**: Shows student account details.
- **User Edit Details**: Allows students to edit their account details.

### Pages for Instructors:

- **Dashboard**: Overview of courses, ratings, and feedback.
- **Insights**: Detailed insights into course views, clicks, and other metrics.
- **Course Management Pages**: Create, update, and delete courses, manage content and pricing.

### Pages for Admin (Future Scope):

- **Dashboard**: Overview of platform courses, instructors, and students.
- **Insights**: Detailed platform metrics.
- **Instructor Management**: Manage instructor details, courses, and ratings.

### Technologies Used:

- **ReactJS**: For building user interfaces.
- **CSS and Tailwind**: For styling.
- **Redux**: For state management.
- **VSCode**: For development.

## Back-end 🛠️

### Description:

StudyNotion uses a monolithic architecture built using Node.js and Express.js, with MongoDB as the primary database.

### Features and Functionalities:

- **User Authentication and Authorization**: Sign up, log in, OTP verification, and password reset.
- **Course Management**: Create, read, update, and delete courses, manage content and media.
- **Payment Integration**: Razorpay for handling payments.
- **Cloud-based Media Management**: Cloudinary for storing and managing media content.
- **Markdown Formatting**: For easier display and rendering of document content.

### Technologies Used:

- **Node.js**: Primary framework for the back end.
- **MongoDB**: Primary database.
- **Express.js**: Web application framework.
- **JWT**: For authentication and authorization.
- **Bcrypt**: For password hashing.
- **Mongoose**: ODM library for MongoDB.

### Data Models and Database Schema:

- **Student Schema**: Fields like name, email, password, and course details.
- **Instructor Schema**: Fields like name, email, password, and course details.
- **Course Schema**: Fields like course name, description, instructor details, and media content.

Overall, the back-end of StudyNotion is designed to provide a robust and scalable solution for an ed-tech platform, with a focus on security, reliability, and ease of use. By using the right frameworks, libraries, and tools, we can ensure that the platform functions smoothly and provides an optimal user experience for all its users.

<!-- How to make this image in the center ? -->

![Data Model](/src/assets/Images/Picture3.jpg)

## API Design 🔌

The API follows the REST architectural style, implemented using Node.js and Express.js, with JSON for data exchange.

### Sample API Endpoints:

1. **POST /api/auth/signup** - Create a new user (student or instructor) account.
2. **POST /api/auth/login** - Log in and generate a JWT token.
3. **POST /api/auth/verify-otp** - Verify the OTP sent to the user's email.
4. **POST /api/auth/forgot-password** - Send a password reset link to the registered email.
5. **GET /api/courses** - Get a list of all available courses.
6. **GET /api/courses/:id** - Get details of a specific course by ID.
7. **POST /api/courses** - Create a new course.
8. **PUT /api/courses/:id** - Update an existing course by ID.
9. **DELETE /api/courses/:id** - Delete a course by ID.
10. **POST /api/courses/:id/rate** - Add a rating to a course.

### Sample API Requests and Responses:

- **GET /api/courses**:
  - **Response**: A list of all courses in the database.
- **GET /api/courses/:id**:
  - **Response**: The course with the specified ID.
- **POST /api/courses**:
  - **Request**: Course details in the request body.
  - **Response**: The newly created course.
- **PUT /api/courses/:id**:
  - **Request**: Updated course details in the request body.
  - **Response**: The updated course.
- **DELETE /api/courses/:id**:
  - **Response**: A success message indicating that the course has been deleted.

## Deployment 🚀

The deployment process involves hosting the application on various cloud-based services.

- **Front-end**: Deployed using Vercel.
- **Back-end**: Hosted on Render or Railway.
- **Media Files**: Hosted on Cloudinary.
- **Database**: Hosted on MongoDB Atlas.

## Future Enhancements 🔮

Potential future improvements:

- **Gamification Features**: Increase user engagement and motivation (Medium Priority).
- **Personalized Learning Paths**: Tailored learning experiences for students (High Priority).
- **Social Learning Features**: Enhance student engagement and interaction (Medium Priority).
- **Mobile App**: More convenient access to the platform (High Priority).
- **Machine Learning-Powered Recommendations**: Improve student engagement (Medium to High Priority).
- **VR/AR Integration**: Enhance the learning experience (Low to Medium Priority).

## Conclusion 🏁

This document outlines the architecture, features, and functionalities of the StudyNotion ed-tech platform, highlighting the use of MERN stack technologies, REST API design, and the deployment process using various hosting services. Additionally, it lists potential future enhancements to improve the platform.

Throughout the development of the project, various achievements will be made in terms of implementing desired functionalities and creating a user-friendly interface. Challenges may arise, such as integrating different technologies and debugging errors, but these will be addressed to ensure the platform's success.

By following best practices in software development, such as code reviews, testing, and documentation, the StudyNotion platform will be a robust and reliable solution for students and instructors alike. The platform aims to revolutionize the ed-tech industry by providing an interactive and engaging learning experience for all users.

---

## Note:

This project is Still in Development phase and thatsWhy there is no attached link for its live working but it will soon be added. So stay Tuned.
For now you can check the code and design of the project.
