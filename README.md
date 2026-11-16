
# Team Collaboration Board

> IFQ636 Software Lifecycle Management Assignment Project

[![CI Pipeline Status](https://github.com/YOUR-USERNAME/YOUR-REPOSITORY/actions/workflows/ci.yml/badge.svg)](https://github.com/YOUR-USERNAME/YOUR-REPOSITORY/actions)

---

# 1. Project Overview

The Team Collaboration Board is a full-stack web application developed using the MERN stack (MongoDB, Express.js, React.js, and Node.js).

The system provides a centralised platform for software development teams to collaborate, organise development activities, manage tasks, track Product Backlog Items (PBIs), and monitor sprint progress using Agile/Scrum methodologies.

Developers can view assigned tasks, update task statuses, manage workloads, and collaborate towards sprint goals. Project administrators can manage team members, create and prioritise PBIs, allocate development tasks, and oversee sprint planning and progress through a dedicated project management dashboard.

The project was developed as part of IFQ636 Software Lifecycle Management and demonstrates software engineering practices including requirements analysis, UI/UX design, Agile project management, version control, CI/CD automation, cloud deployment, and software testing.

---

# 2. Features

## Developer Features

- Register a new account
- Login and logout securely
- View personal developer dashboard
- View assigned development tasks
- Update task status (To Do, In Progress, Completed, Blocked)
- View task priorities and deadlines
- View associated Product Backlog Items (PBIs)
- Track current sprint progress
- View sprint goals and timelines
- Monitor individual workload
- Update user profile

## Admin / Project Manager Features

- Manage developer accounts
- Create, edit, and manage development tasks
- Assign tasks to developers
- Set task priorities and deadlines
- Create and manage Product Backlog Items (PBIs)
- Define PBI descriptions and acceptance criteria
- Allocate story points
- Prioritise the product backlog
- Create and manage sprints
- Define sprint goals and durations
- Monitor sprint progress and completion
- Track developer workloads
- View project activity and performance

---

# 3. Technology Stack

## Frontend

- React.js
- React Router
- Bootstrap 5
- Tailwind CSS
- Axios

## Backend

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- JWT Authentication

## DevOps and Tools

- GitHub
- GitHub Actions
- AWS EC2 Ubuntu
- Jira
- Figma

---

# 4. System Architecture

The Team Collaboration Board follows a three-tier architecture.

- **Frontend:** React.js provides the user interface for developers and administrators.
- **Backend:** Node.js and Express.js provide REST API endpoints for authentication, task management, PBI management, and sprint management.
- **Database:** MongoDB Atlas stores user accounts, developer tasks, Product Backlog Items, sprint information, and project data.

### Core System Modules

1. User Authentication and Authorisation
2. Developer and Team Management
3. Task Management
4. Product Backlog Management
5. Sprint Planning and Tracking
6. Project Dashboard and Reporting

---

# 5. Git Branching Strategy

GitHub is used for source code management and collaborative development.

The following branching strategy is implemented:

- **Feature Branch:** Used to develop individual features and functionalities.
- **Develop Branch:** Integrates completed features for development and testing.
- **Release Branch:** Used to prepare and validate application releases.
- **Main Branch:** Contains the stable production-ready application.

Pull requests are used to review and merge changes between branches, supporting collaborative development and code quality.

---

# 6. CI/CD Pipeline

GitHub Actions is used to automate build validation, testing, and deployment.

### Deployment Flow

- Feature Branch
- Develop Branch
- Release Branch
- Main Branch
- GitHub Actions Workflow
- AWS EC2 Deployment

### Pipeline Activities

- Checkout the latest repository code
- Install project dependencies
- Run automated validation and tests
- Build the React frontend
- Deploy the latest application code to AWS EC2
- Restart backend services
- Restart frontend services

---

# 7. Local Setup

## 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

## 2. Install Dependencies

```bash
npm install
npm install --prefix backend
npm install --prefix frontend
```

## 3. Configure Environment Variables

### Backend (.env)

```env
PORT=5001
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### Frontend (.env)

```env
REACT_APP_API_URL=http://localhost:5001/api
```

## 4. Run the Application

### Start Backend

```bash
npm start --prefix backend
```

### Start Frontend

```bash
npm start --prefix frontend
```

---

# 8. Public Project URL

### Live Application

```text
http://YOUR-EC2-PUBLIC-IP
```

Replace the URL above with your deployed AWS EC2 public IP address.

---

# 9. Test Login Details

## Admin / Project Manager Account

Email: YOUR_ADMIN_EMAIL

Password: YOUR_ADMIN_PASSWORD

## Developer Account

Email: YOUR_DEVELOPER_EMAIL

Password: YOUR_DEVELOPER_PASSWORD

Replace the placeholder credentials with the test accounts configured for the application.

---

# 10. Deployment

The application is deployed using:

- AWS EC2 Ubuntu Server
- MongoDB Atlas
- GitHub Actions
- GitHub Self-Hosted Runner
- PM2 Process Manager

GitHub Actions automates application validation and deployment to the AWS EC2 instance.

PM2 is configured to manage application processes and automatically restart services when required. The PM2 process configuration is saved to support application recovery following an EC2 instance restart.

---

# 11. Project Structure

```text
team-collaboration-board/
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   └── server.js
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── services/
│   │   └── App.js
│   └── build/
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── README.md
└── package.json
```

---

# 12. Testing

The following testing activities are included in the project testing scope:

- User Authentication Testing
- Role-Based Access Control Testing
- Developer Task CRUD Testing
- Task Assignment and Status Update Testing
- Product Backlog Item (PBI) Management Testing
- Sprint Creation and Management Testing
- Sprint Progress Tracking Testing
- Developer Workload Testing
- API Testing using Postman
- GitHub Actions Pipeline Testing
- AWS Deployment Testing

---

# 13. Project Artefacts

This project includes:

- Requirements Analysis
- Stakeholder Analysis
- SysML Diagrams
- Jira Project Board
- Product Backlog and User Stories
- Sprint Planning and Management
- Low-Fidelity UI/UX Wireframes
- High-Fidelity Figma Prototype
- GitHub Repository
- CI/CD Pipeline
- AWS Cloud Deployment
- Software Testing Documentation

---

# 14. Author

**YOUR NAME**

Master of Information Technology

Queensland University of Technology (QUT)

IFQ636 Software Lifecycle Management

2026
