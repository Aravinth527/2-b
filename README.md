# Node File Upload Server

This project is a simple Node.js application that allows users to upload files through a web interface. It uses the Express framework and Multer middleware for handling file uploads.

## Installation Steps
1. Run `npm init -y` to create a package.json file.
2. Install dependencies with `npm install express multer`.
3. Create the "uploads" directory in the project root.

## Instructions to Run the Server
1. Navigate to the project directory.
2. Run the server using `node src/index.js`.
3. Open a web browser and go to `http://localhost:3000` to access the file upload interface.

## Step-by-Step Explanation
- The server listens on port 3000 and serves the HTML file upload form at the root route.
- When a file is uploaded via the form, the POST /upload route is triggered, where Multer processes the file and saves it to the "uploads" directory.
- The GET /files route retrieves and lists all uploaded files, returning their filenames in JSON format.