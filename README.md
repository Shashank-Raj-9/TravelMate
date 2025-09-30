## TravelMate Web Project Installation Guide

This guide will walk you through the installation process for the TravelMate web project. Follow the steps below to set up the project locally on your machine.

## Prerequisites

Before you begin, make sure you have the following installed on your system:

Node.js (version 18 recommended)

MongoDB

Nodemon (installed globally)

## Installation Steps
1. Clone the TravelMate repository from GitHub:

 git clone https://github.com/Shashank-Raj-9/TravelMate.git

2. Set up the database:

Create a .env file in the root directory of the project.

Add the following line to the .env file:

ATLASDB_URL=mongodb://127.0.0.1:27017/travelmate


You can change the database name travelmate if you prefer.

3. Set up Cloudinary:

Go to Cloudinary
 and sign up for a free account.

Obtain your Cloudinary credentials: CLOUD_NAME, CLOUD_API_KEY, and CLOUD_API_SECRET.

Add these values to your .env file:

CLOUD_NAME=your_cloud_name
CLOUD_API_KEY=your_api_key
CLOUD_API_SECRET=your_api_secret

4. Set the secret key for Cloudinary storage:
SECRET=your_cloudinary_secret


Use a strong and secure value for SECRET.

5. Install project dependencies:
npm install

6. Seed the database with sample listings (optional but recommended):
node init/index.js


This will populate the database with sample travel listings so you can explore the app immediately.

7. Run the application using Nodemon:
nodemon app.js


The server should start on port 8080.

8. Access the project:

Open your browser and go to:

http://localhost:8080

You should see the TravelMate listings with photos, descriptions, and pricing.

✅ Notes:

You only need to run node init/index.js once to seed the database.

Later, you can add new listings via the app.

Make sure MongoDB is running locally before starting the app.

Happy traveling with TravelMate! 🌍✈️