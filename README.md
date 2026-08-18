# 🍱 ResQBite – Food Donation & NGO Coordination Platform

ResQBite is a **full-stack mobile application** designed to reduce food wastage by connecting **food donors, NGOs, and volunteers**. The platform enables donors to share surplus food, NGOs to coordinate collection and distribution, and volunteers to help bridge the gap between donors and organizations.

The project focuses on using technology to make surplus-food redistribution more organized, accessible, and efficient.

## 🎯 Problem Statement

Large quantities of edible food are wasted while many people and organizations struggle to access sufficient food resources. ResQBite aims to address this gap by providing a centralized platform where surplus food can be listed and coordinated for redistribution.

## ✨ Key Features

### 👤 Role-Based Platform

* Separate workflows for **Donors, NGOs, and Volunteers**
* Role-based access control for protected functionality
* Secure user authentication

### 🍱 Food Donation Management

* Create and manage food donation requests
* Track donation details and status
* Upload images of donated food
* Store relevant donation information securely

### 🔐 Authentication & Authorization

* JWT-based authentication
* Role-based authorization
* Protected API routes
* Secure user sessions

### ☁️ Image Management

* Cloudinary integration for food-image uploads
* Cloud-based image storage and management

### 📱 Mobile Application

* Built using React Native and Expo
* Reusable and responsive components
* Mobile-friendly user experience
* Frontend-backend API integration

## 🏗️ System Architecture

```text
┌──────────────────────────┐
│      React Native        │
│      Mobile App          │
└────────────┬─────────────┘
             │ REST APIs
             ▼
┌──────────────────────────┐
│    Node.js + Express     │
│       Backend API        │
└───────┬───────────┬──────┘
        │           │
        ▼           ▼
┌─────────────┐  ┌─────────────┐
│   MongoDB   │  │  Cloudinary │
│  Database   │  │    Images   │
└─────────────┘  └─────────────┘
```

## 🛠️ Tech Stack

**Frontend**

* React Native
* Expo

**Backend**

* Node.js
* Express.js
* REST APIs

**Database**

* MongoDB

**Authentication**

* JSON Web Tokens (JWT)

**Cloud Services**

* Cloudinary

**Development Tools**

* Git
* GitHub
* Postman

## 📂 Project Structure

```text
ResQBite/
│
├── frontend/
│   ├── app/
│   ├── components/
│   ├── screens/
│   └── ...
│
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── config/
│   └── server.js
│
├── README.md
└── ...
```

> The exact structure may vary depending on the current repository version.

## 🚀 Getting Started

### Prerequisites

Make sure you have installed:

* Node.js
* npm
* MongoDB
* Expo CLI / Expo Go
* Git

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd ResQBite
```

### 2. Install backend dependencies

```bash
cd backend
npm install
```

### 3. Configure environment variables

Create a `.env` file in the backend directory:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

Never commit your `.env` file or expose secret credentials publicly.

### 4. Start the backend

```bash
npm start
```

For development:

```bash
npm run dev
```

### 5. Start the mobile application

From the frontend directory:

```bash
npm install
npx expo start
```

Then open the application using Expo Go or an available emulator.

## 🔄 Application Flow

```text
User Registration/Login
        ↓
    Select Role
        ↓
┌───────┼────────┐
↓       ↓        ↓
Donor   NGO   Volunteer
 ↓
Create Donation
 ↓
Upload Food Image
 ↓
Submit Donation
 ↓
Donation Management
```

## 🔒 Security

* JWT-based authentication
* Role-based authorization
* Protected API endpoints
* Backend validation
* Environment variables for sensitive credentials

## 🌱 Future Improvements

* Real-time notifications for donation requests
* Location-based donor/NGO matching
* Donation pickup scheduling
* Food expiry tracking
* Analytics dashboard
* Improved NGO and volunteer workflows

## 👩‍💻 My Contribution

I contributed to the development of the application with a focus on:

* Building the **Donor Dashboard**
* Developing RESTful APIs using Node.js and Express.js
* Implementing JWT authentication and role-based authorization
* Integrating MongoDB for application data
* Integrating Cloudinary for image management
* Connecting the React Native frontend with backend APIs
* Developing reusable mobile UI components
* Implementing validation and error handling

## 📌 Project Status

**Academic / Portfolio Project**

The project was developed as a full-stack mobile application to demonstrate practical software engineering, backend development, database integration, authentication, and mobile application development skills.
