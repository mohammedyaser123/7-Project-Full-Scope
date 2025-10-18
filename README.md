# 7-Project-Full-Scope
Job Finder Web Application
Project Overview
The Job Finder web application was developed to solve a real-world problem — bridging the gap between job seekers and employers. Many people struggle to find suitable opportunities, while employers often have difficulty reaching the right candidates. This platform simplifies that process by providing an intuitive interface for both groups.
Job seekers can create accounts, search for available positions by job title, location, or salary range, and apply directly. Employers can register, post new job listings, and manage their existing openings efficiently. The goal of the project is to make connecting job seekers and employers as seamless and effective as possible.

Setup Instructions
1. Prerequisites
Make sure the following are installed on your system:
•	Node.js (https://nodejs.org/en/download)
•	MongoDB (local installation or a cloud instance via MongoDB Atlas)

2. Open the Project
1.	Open the main project folder (for example, job-finder) in Visual Studio Code.
2.	Ensure the project contains two folders:
o	server — backend (API, database, authentication)
o	client — frontend (user interface)

3. Run the Server
1.	In the integrated terminal, navigate to the server folder:
2.	cd server
3.	Install backend dependencies:
4.	npm install
5.	Set up your environment variables:
o	Create a .env file inside the server directory and add:
o	MONGO_URI=your_mongodb_connection_string
o	JWT_SECRET=your_secret_key
o	PORT=5000
6.	Start the server:
7.	npm run dev
The server should start on http://localhost:5000.

4. Run the Client
1.	Open a new terminal window and navigate to the client folder:
2.	cd client
3.	Install frontend dependencies:
4.	npm install
5.	Start the React client:
6.	npm start
The client will start on http://localhost:3000.

5. Connecting Client and Server
•	If you are using Create React App, add the following line to your client/package.json file:
•	"proxy": "http://localhost:5000"
This allows the frontend to communicate with the backend API without specifying full URLs.
•	If you are using Vite, create a .env file in the client folder with:
•	VITE_API_BASE=http://localhost:5000

6. Run the Full Application
Once both servers are running:
•	Open your browser and go to http://localhost:3000.
•	Register as a job seeker or employer.
•	Explore job listings, post new jobs, and test full CRUD operations.

7. Key Technologies
•	React (frontend)
•	Node.js and Express (backend)
•	MongoDB with Mongoose (database)
•	JWT (authentication)
•	Axios (API requests)
•	Tailwind CSS or Bootstrap (styling)

