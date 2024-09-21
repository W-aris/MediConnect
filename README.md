# MediConnect 🏥 by Mohammad Waris

**MediConnect** is a comprehensive healthcare platform designed to connect users with healthcare professionals seamlessly. This project offers a robust, secure, and user-friendly interface for both patients and doctors, allowing easy appointment management, profile updates, and more. Administrators are equipped with powerful tools to manage users, doctors, and appointments efficiently.

## 🌟 Project Overview

MediConnect aims to simplify healthcare interactions by providing an integrated platform for:

- **Patients**: Book appointments, manage profiles, and get updates.
- **Doctors**: Manage patient appointments, update profiles, and track schedules.
- **Administrators**: Oversee platform operations, approve doctor applications, and ensure smooth functionality.

## 🔧 Key Features

- **User Registration & Login**: Patients and doctors can register and securely log in.
- **Doctor Listings**: Browse and select from available doctors based on specialties.
- **Appointment Booking**: Patients can book appointments with doctors, and appointments can be tracked.
- **Admin Dashboard**: Manage users, approve or reject doctor applications, and maintain platform integrity.
- **Notifications**: Get real-time notifications about appointments and application status.
- **Profile Management**: Keep user profiles updated with relevant information.
- **Doctor Applications**: Doctors can apply to be listed on the platform and get approved by the admin.

## 🛠️ Tools and Technologies

- **Backend**: Node.js, Express.js
- **Frontend**: React.js, Redux
- **Database**: MongoDB for storing all user and doctor information securely.


## 🗃️ Database Setup (MongoDB)

To set up MongoDB, follow these steps:

1. **Create a MongoDB Account**  
   - Visit [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register) and create a free account.
   - Set up a new cluster by following the instructions.

2. **Create a Database**  
   - After setting up your cluster, click on "Collections" and then "Create Database."
   - Name your database (e.g., `mediconnect_db`) and create your collections (e.g., `users`, `doctors`, `appointments`).

3. **Update `.env` File**  
   - Rename `.env.example` to `.env` in the project root folder.
   - Add your MongoDB connection string in the `.env` file as shown below:
     ```
     MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/<dbname>?retryWrites=true&w=majority
     ```

4. **Running the Database**  
   - Run the project locally and ensure the backend connects to MongoDB successfully using the above configuration.

## 🚀 Running the Project Locally

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/en/)
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register) for a remote database
- [Git](https://git-scm.com/)

### Steps to Run

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/MediConnect.git
   cd MediConnect
   ```

2. **Install Dependencies**
   In the project root folder, run:
   ```bash
   npm install
   ```

3. **Setup Environment Variables**
   - Rename the `.env.example` file to `.env`.
   - Add the necessary environment variables such as `MONGO_URI`, `PORT`, etc.

4. **Start the Backend**
   In the root directory, run:
   ```bash
   npm start
   ```

5. **Start the Frontend**
   Navigate to the `client` folder and run:
   ```bash
   cd client
   npm start
   ```

The app should now be running on `localhost` with both the backend and frontend servers active.

## 🌐 Live Deployment

You can access the live version of the MediConnect platform [here](https://mediconnect.onrender.com).

## ⚠️ Challenges Faced

During the development of MediConnect, several challenges were encountered:

- **Database Connection Issues**: Initial attempts to connect to MongoDB failed due to improper environment variable configurations. This was solved by carefully debugging the `.env` file and ensuring the MongoDB URI was correct.
- **Data Consistency**: Ensuring consistent data flow between different components (user, doctor, and admin roles) was a significant challenge, but using Redux for state management helped overcome this.
- **Deployment**: Deploying the app on Render.com required specific configurations, especially with environment variables for MongoDB.

## 📂 Project Structure

```bash
HealthBooker-main/
│
├── client/               # React frontend
├── controllers/          # Backend controllers
├── db/                   # Database connection configuration
├── middleware/           # Express middlewares
├── models/               # MongoDB models
├── routes/               # API routes
├── server.js             # Main server file
├── .env.example          # Example environment file
├── package.json          # Backend dependencies
└── README.md             # Project documentation
```

## 🛡️ License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## 🧑‍💻 Contributors

- **Waris** (Lead Developer)

