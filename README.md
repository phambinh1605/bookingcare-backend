🏥 Doctor Appointment Booking - Backend

📌 Overview
This is the backend of the "Doctor Appointment Booking" web application. It is built using Node.js with Express, and connects to a MySQL database to manage data related to patients, doctors, clinics, and appointment schedules.

⚙️ Technologies Used

Node.js: JavaScript runtime environment for building server-side applications.

Express: Web framework for handling APIs and routing.

MySQL: Relational database for storing application data.

Sequelize: ORM for interacting with the MySQL database.

🚀 Installation Guide

1. Clone the repository:

    git clone https://github.com/username/backend-repo.git

2. Install dependencies:

    cd backend-repo

    npm install

3. Environment setup:

• Copy the .env.example file and create a new file named .env in the root folder.

• Update the following environment variables in the .env file:

    DB_USERNAME     // Your MySQL username (default: root)

    DB_PASSWORD     // Your MySQL password

    MAIL_USERNAME   // Your email address

    MAIL_PASSWORD   // App-specific password (not your email login password)

To generate a mail app password (Gmail):

    https://myaccount.google.com/apppasswords

4. Database setup:

• Use MySQL Workbench or PHPMyAdmin to run the database.sql file located in the database/ folder.

• This will automatically create a schema named doctorcare.

5. Run the server:

    npm start

The backend server will run at:

    📍 http://localhost:8080
    
📚 API Endpoints

• GET /api/doctors — Get list of doctors

• POST /api/appointments — Book an appointment

• GET /api/appointments — Get patient’s appointment list

• GET /api/patients — Get patient information

📁 Project Structure

    📂 controllers/   // Handles business logic for APIs

    📂 models/        // Sequelize models (User, Doctor, Appointment)

    📂 routes/        // Defines API endpoints and routes

    📂 config/        // Database config and other settings
    
🐞 Common Issues

1. Database not connecting

• Check your .env configuration

• Ensure MySQL server is running

2. API not responding

• Verify endpoint URLs in routes/

• Use tools like Postman to test responses


