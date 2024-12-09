# FusionHub
# **FusionHub - A Comprehensive Project and Portfolio Management Platform**

FusionHub is a modern project and portfolio management application designed for students and administrators. It combines powerful tools for managing projects, teams, and personal portfolios, along with robust user management capabilities for administrators.

---

## **Key Features**

### **Student Features**
1. **Discover and Search Projects**  
   - Browse and filter projects using various criteria to find relevant ones quickly.  

2. **Create and Manage Projects**  
   - Start a new project and invite team members via email.  
   - Assign roles and manage team collaborations.  

3. **Kanban-Style Task Management**  
   - Create, assign, and track tasks for each project.  
   - Tasks can be moved across different statuses: **To-Do**, **Pending**, and **Done**.  
   - Add comments and updates to tasks to streamline communication.  

4. **Real-Time Chat**  
   - Collaborate effectively with team members using integrated real-time chat functionality.  

5. **Project Progress Tracking**  
   - Monitor the overall progress of each project using detailed metrics and visualizations.  

6. **Issue Management**  
   - Create and assign issues to team members.  
   - Track the progress of issues and add comments to facilitate resolution.  

7. **Portfolio Creation**  
   - Build a personalized portfolio with:  
     - Customizable themes.  
     - Sections for experience, education, social links, and an "About Me" page.  
     - Toggle visibility of specific projects.  
   - Shareable portfolio link for showcasing achievements.  

8. **Profile Management**  
   - Create and update user profiles, including personal details and preferences.  
   - Reset forgotten passwords using the **Forgot Password** feature.  

9. **Authentication and Security**  
   - Secure login with JWT-based authentication and Spring Security.  
   - OAuth 2.0 login via Google for seamless access.  

---

### **Admin Features**
1. **User Management**  
   - View a list of users with their names, email addresses, and login sources (FusionHub or Google).  

2. **User Status Management**  
   - Admin can approve or reject user registrations:  
     - **FusionHub Signup:** User status is set to "Pending" and requires admin approval.  
     - **Google Signup:** Automatically approved, but the admin can later change the status.  

3. **Comprehensive Control Panel**  
   - Easily manage users, projects, and portfolios from a centralized dashboard.  

---

## **Tech Stack**

### **Backend**
- **Spring Boot** for building robust REST APIs.
- **JWT and Spring Security** for authentication and authorization.
- **MySQL** as the database for storing user, project, and portfolio data.

### **Frontend**
- **React.js** for creating a dynamic and responsive user interface.


### **Real-Time Communication**
- **WebSocket** for enabling real-time chat and updates.

### **OAuth Integration**
- **Google OAuth 2.0** for secure and streamlined login functionality.

### **DevOps and CI/CD**
- **GitHub Actions** for continuous integration and automated submodule updates.

---

## **How It Works**

### **For Students**
- **Project Management**: Students can create and manage projects, assign tasks, and track progress with ease.  
- **Portfolio Creation**: Build stunning portfolios to showcase skills and achievements.  
- **Collaboration**: Use real-time chat and task management to stay connected with team members.  

### **For Admins**
- **User Control**: Monitor user activities and approve or reject user registrations.  
- **Security**: Ensure safe and controlled access to the platform.  

---




---  

## **FusionHub Project Setup Guide**

This document explains how to set up and run the FusionHub project locally or in a production environment. Follow the steps below to get started.

---

## **Project Structure**
 ```
 FusionHub/
├── Backend/
│   ├── AdminService/
│   ├── StudentService/
│   ├── EurekaServer/
│   └── APIGateway/
├── Frontend/
└── README.md

```
Each service is self-contained and can be developed/tested independently.


---

## **Setup Instructions**

### **1. Prerequisites**
Ensure the following tools are installed on your system:
- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) (version 11 or later)
- [Node.js](https://nodejs.org/) and npm (for the frontend)
- [Maven](https://maven.apache.org/download.cgi) (for backend services)
- [Git](https://git-scm.com/) (for cloning the repository and managing submodules)
- A database (e.g., MySQL) configured for backend services.

---

### **2. Clone the Main Repository**
Clone the main repository along with its submodules:
```bash
git clone --recursive https://github.com/manishraj27/FusionHub.git
cd FusionHub
```

If you cloned without the --recursive flag, initialize and update the submodules manually:

```
git submodule init
git submodule update
```

### 3. Configure Environment Variables
Each service requires environment variables for configuration in application.properties.

### 4. Build and Run Frontend
Navigate to the Frontend directory:
```
cd Frontend
```

Install dependencies:
```
npm install
```

Start the development server:
```
npm run dev
```
### 5. Start the backend SpringBoot Project
- APIGateway
- EurekaServer
- StudentService
- AdminService
