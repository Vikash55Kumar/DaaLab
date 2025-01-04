# DAA Virtual Lab

## Overview
DAA Virtual Lab is a comprehensive web-based platform developed to facilitate seamless student and teacher interactions within an academic environment. The project enables teachers to manage assignments, track student progress, and oversee real-time activity, while students can efficiently submit their work and monitor their performance. This application supports the effective digital transformation of educational workflows.

---

## Features

### For Students:
- **Assignment Management**: View assignments specific to their section with details like due dates and descriptions.
- **Progress Tracking**: Track submitted work and its status (e.g., Pending, Completed).
- **Profile Dashboard**: Personalized dashboard to monitor academic progress.
- **Submission**: Submit assignments with file uploads and track submission dates.

### For Teachers:
- **Dashboard**: Manage and monitor assignments across multiple sections.
- **Assignment Creation**: Create, edit, and schedule assignments for specific sections.
- **Student Progress Tracking**: View individual student progress and status of submitted work.
- **Real-Time Activity Monitoring**: Track real-time activities of students and teachers.

### For Admins:
- **User Management**: Register and manage teachers and students.
- **Activity Logs**: Monitor system activity and user actions.
- **Section Management**: Create and manage sections with assigned students and teachers.

---

## Tech Stack

### Frontend:
- **Framework**: React.js
- **Styling**: TailwindCSS
- **State Management**: Redux

### Backend:
- **Framework**: Node.js with Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)

### Tools:
- **Version Control**: Git & GitHub
- **Hosting**: AWS EC2 and S3
- **Package Management**: NPM (Node Package Manager)

## Installation and Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/username/DAA-Virtual-Lab.git
   ```

2. **Install Dependencies:**
   ```bash
   cd DAA-Virtual-Lab
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root directory and add the following:
   ```
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   ACCESS_TOKEN_SECRET=your_access_token_secret
   REFRESH_TOKEN_SECRET=your_refresh_token_secret
   ```

4. **Run the Application:**
   ```bash
   npm start
   ```

5. **Access the Application:**
   Open your browser and navigate to `http://localhost:5000`.

---

## Data Flow

### 1. Authentication Flow:
   - **Login**: User submits credentials, verified against the database.
   - **Token Generation**: JWT tokens issued for session management.

### 2. Assignment Flow:
   - **Teacher**: Creates an assignment and assigns it to a section.
   - **Student**: Views the assignment, submits work, and updates status.
   - **Database**: Tracks assignment status and submissions.

### 3. Progress Tracking:
   - Fetches data from `StudentWork` schema and displays it on dashboards for both students and teachers.

---

## Future Enhancements
- **Real-Time Notifications**: Notify users about assignment updates and deadlines.
- **Gradebook Integration**: Allow teachers to grade assignments directly.
- **Enhanced Analytics**: Provide detailed insights into student performance.
- **Mobile App**: Extend platform availability with a cross-platform mobile application.

---

## Contributing

We welcome contributions! Please follow these steps:
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push to your fork.
5. Create a Pull Request.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact

For questions or collaboration, feel free to reach out:
- **Email**: vikash@example.com
- **GitHub**: [Vikash](https://github.com/username)
