Blog Application

This is a full-stack blog application built with Node.js, Express, and EJS. It allows users to create, read, update, and delete blog posts through a RESTful API and a web interface. The application consists of two main components:





Backend API (index.js): Manages blog post data with CRUD operations using an in-memory data store.



Frontend Server (server.js): Serves EJS templates for the user interface and communicates with the backend API.

Features





View a list of all blog posts.



Create new blog posts.



Edit existing blog posts.



Delete blog posts.



RESTful API for managing posts.

Prerequisites





Node.js (v14 or higher)



npm (comes with Node.js)



A web browser to access the application

Installation





Clone the repository:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name



Install dependencies: Navigate to the project directory and install the required Node.js packages:

npm install

This will install express, body-parser, axios, and ejs.



Directory Structure: Ensure your project has the following structure:

your-repo-name/
├── public/
│   └── (static files: CSS, JS, etc.)
├── views/
│   ├── index.ejs
│   └── modify.ejs
├── index.js
├── server.js
├── package.json
└── README.md

Running the Application





Start the Backend API: Run the index.js file to start the API server on port 4000:

node index.js

You should see: API is running at http://localhost:4000.



Start the Frontend Server: In a separate terminal, run the server.js file to start the frontend server on port 3000:

node server.js

You should see: Backend server is running on http://localhost:3000.



Access the Application: Open your browser and navigate to http://localhost:3000 to view the blog application.

Usage





Home Page (/): Displays a list of all blog posts.



Create Post (/new): Navigate to this route to create a new blog post.



Edit Post (/edit/:id): Edit an existing post by its ID.



Delete Post (/api/posts/delete/:id): Delete a post by its ID.



API Endpoints:





GET /posts: Retrieve all posts.



GET /posts/:id: Retrieve a specific post by ID.



POST /posts: Create a new post.



PATCH /posts/:id: Update a post by ID.



DELETE /posts/:id: Delete a post by ID.

Dependencies





express: Web framework for Node.js.



body-parser: Middleware to parse incoming request bodies.



axios: Promise-based HTTP client for making API requests.



ejs: Templating engine for rendering dynamic HTML.

Notes





The application uses an in-memory data store (posts array in index.js), so data will reset when the server restarts. For persistent storage, consider integrating a database like MongoDB or PostgreSQL.



Ensure both servers (index.js and server.js) are running simultaneously for the application to function correctly.



The public folder should contain any static assets (e.g., CSS, JavaScript) used by the EJS templates.



The views folder must contain index.ejs and modify.ejs templates for rendering the UI.

Contributing





Fork the repository.



Create a new branch (git checkout -b feature-branch).



Make your changes and commit (git commit -m "Add feature").



Push to the branch (git push origin feature-branch).



Create a pull request.

License

This project is licensed under the MIT License. See the LICENSE file for details.
