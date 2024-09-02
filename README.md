Express Authentication App A simple Express.js application for user authentication with signup and login functionality. This app uses EJS for templating, bcrypt for password hashing, and connects to a MongoDB database for storing user data.

Features User signup with validation User login with password hashing Basic error handling and validation Static files served from the public directory Installation Clone the repository:

bash Copy code git clone https://github.com/yourusername/your-repo.git cd your-repo Install dependencies:

Ensure you have Node.js and npm installed. Then run:

bash Copy code npm install Set up your MongoDB database:

Make sure MongoDB is installed and running.

Create a .env file in the root directory of your project with the following content (update with your actual MongoDB connection string):

env Copy code MONGO_URI=mongodb://localhost:27017/your-database Start the server:

bash Copy code npm start The server will run on http://localhost:3000.

Usage Homepage: http://localhost:3000/ - Displays the login page. Signup: http://localhost:3000/signup - Displays the signup page. Login: http://localhost:3000/login - Displays the login page. API Endpoints POST /signup - Create a new user. Requires username, password, confirmpassword, email, phone, and dob. POST /login - Authenticate a user. Requires username and password. Error Handling Returns appropriate status codes and error messages for missing fields, mismatched passwords, invalid password format, or existing users. Dependencies express - Web framework path - Module for path operations ejs - Templating engine body-parser - Middleware to parse request bodies bcrypt - Library for hashing passwords mongoose - MongoDB object modeling tool (assumed to be used in src/mongodb.js) Contributing Feel free to open issues or submit pull requests. Please make sure to follow the coding style and write meaningful commit messages.

License This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments Express - Web framework EJS - Templating engine bcrypt - Password hashing MongoDB - NoSQL database
