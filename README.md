# Blood Donation Management Web App

## Overview
The Blood Donation Management Web App is designed to facilitate the process of blood donation by connecting donors, moderators, and administrators in a secure and efficient platform. The app allows users to view, post, and manage blood donation requests in real-time. It utilizes Next.js for the frontend, React.js for the user interface, and Firebase for authentication and backend management. With Role-Based Access Control (RBAC), users are assigned roles (Donor, Moderator, Admin) that determine their access and functionality within the app.

This platform aims to improve the efficiency of the blood donation process, ensuring that patients receive blood in a timely manner while making it easier for donors to contribute.

## Features

### Role-Based Access Control (RBAC):
- Different roles (Admin, Moderator, Donor) with specific dashboards and functionalities.
  
### Real-Time Blood Donation Requests:
- Donors can view real-time donation requests that match their blood type.
- Moderators can post new donation requests with relevant details.
- Donors receive email notifications for new or updated requests.

### User Dashboards:
- **Donor Dashboard**: View and respond to available blood donation requests.
- **Moderator Dashboard**: Manage blood donation requests and view potential donors.
- **Admin Dashboard**: Full access to user management and system configuration.

### Secure Authentication:
- Firebase Authentication is used to register, log in, and manage user accounts.
- Role-based access ensures users have appropriate permissions.

## Technologies Used

### Frontend:
- **Next.js**: Server-side rendering and optimized performance.
- **React.js**: For building the user interface.

### Backend:
- **Firebase**: Authentication, Firestore Database, Firebase Functions.

### Notifications:
- **Firebase Cloud Messaging**: For real-time email notifications.

### UI/UX:
- Responsive design ensuring compatibility across devices.

## Installation

### Prerequisites:
- Node.js (v16 or higher)
- Firebase account (for Firebase Authentication and Firestore)

### Steps to Install:

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/blood-donation-web-app.git
    cd blood-donation-web-app
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Set up Firebase:
   - Create a Firebase project if you haven't already.
   - Configure Firebase Authentication and Firestore Database.
   - Obtain your Firebase project configuration from the Firebase Console and add it to the project. Place this configuration in `firebaseConfig.js`.

4. Run the development server:

    ```bash
    npm run dev
    ```

5. Access the application:
   - Visit `http://localhost:3000` in your browser to see the app in action.

## Usage

### Donors:
- After signing in, donors can view available blood donation requests that match their blood type and express interest in donating.

### Moderators:
- Moderators can post new blood donation requests, see compatible donors, and manage existing requests.

### Admins:
- Admins can manage users, assign roles, and have full access to the app's configuration and settings.

## Role-Based Access Control (RBAC)
The app uses RBAC to manage permissions for different users:

- **Donor**: Can view blood donation requests and respond to them.
- **Moderator**: Can post new donation requests, view compatible donors, and manage ongoing requests.
- **Admin**: Can manage users, configure roles, and access all platform settings.

