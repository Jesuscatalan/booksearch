# booksearch
take a fully functioning Google Books API search engine built with a RESTful API, and refactor it to be a GraphQL API built with Apollo Server. The app was built using the MERN stack, with a React front end, MongoDB database, and Node.js/Express.js server and API.

📚 Book Search Engine

🚀 Description
The Book Search Engine is a full-stack MERN application that allows users to search for books using the Google Books API. Users can create an account, log in, and save their favorite books to their profile. This project was originally built with a RESTful API and has been refactored to use GraphQL with Apollo Server for improved efficiency.

📌 User Story
As an avid reader,
I want to search for new books to read,
so that I can keep a list of books to purchase.

✅ Features & Acceptance Criteria
Users can search for books using the Google Books API.
Non-logged-in users can view book details but cannot save books.
Logged-in users can save books to their profile.
Users can remove saved books from their list.
Authentication system with JWT (Signup/Login/Logout).
Uses Apollo Server to handle GraphQL queries and mutations.

🛠 Technologies Used
MongoDB Atlas (Database)
Express.js (Backend Framework)
React.js (Frontend)
Node.js (Server)
GraphQL & Apollo Server (API)
JWT Authentication (User Authentication)
TypeScript (for better maintainability)
Mongoose (MongoDB ODM)
Render (Deployment)

⚙️ Installation

1️⃣ Clone the Repository
git clone https://github.com/jesuscatalan/book-search-engine.git
cd book-search-engine

2️⃣ Install Dependencies
npm install

3️⃣ Set Up Environment Variables
Create a .env file in the root directory and add:

ini

MONGODB_URI=your_mongodb_atlas_uri
JWT_SECRET=your_secret_key

4️⃣ Start the Development Server
Backend (GraphQL + Express)
cd server
npm run dev
Frontend (React + Apollo Client)

cd client
npm start


🔗 API & GraphQL Schema
GraphQL Queries & Mutations

🔍 Queries
me: Get logged-in user's profile and saved books.

🔄 Mutations
login(email, password): Logs in a user and returns a token.
addUser(username, email, password): Registers a new user and returns a token.
saveBook(bookId, title, authors, description, image, link): Saves a book to the user's profile.
removeBook(bookId): Removes a saved book from the user's profile.

🚀 Deployment
The application is deployed on Render with a MongoDB Atlas database.

Live App: Deployed Link

📝 License
This project is licensed under the MIT License.

