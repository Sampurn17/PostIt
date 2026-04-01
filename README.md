# PostIt 📝

A simple social posting web application built with **Node.js, Express, MongoDB, and EJS** where users can register, login, create posts, like/unlike posts, and edit their posts.

---

## Features 🚀

* User Registration with password hashing (bcrypt)
* Secure Login using JWT authentication
* Cookie-based session handling
* Create posts
* Edit posts
* Like / Unlike posts
* User profile page showing all posts
* Simple UI built with **TailwindCSS + EJS**

---

## Tech Stack 🛠

**Backend**

* Node.js
* Express.js
* MongoDB
* Mongoose

**Authentication**

* JSON Web Tokens (JWT)
* bcrypt

**Frontend**

* EJS Templates
* Tailwind CSS

**Other**

* cookie-parser

---

## Project Structure 📁

```
PostIt
│
├── models
│   ├── user.js
│   └── post.js
│
├── views
│   ├── index.ejs
│   ├── login.ejs
│   ├── profile.ejs
│   └── edit.ejs
│
├── app.js
├── package.json
└── README.md
```

---

## Installation ⚙️

Clone the repository

```
git clone https://github.com/yourusername/postit.git
```

Go into the project folder

```
cd postit
```

Install dependencies

```
npm install
```

Run the server

```
node app.js
```

Server runs on

```
http://localhost:3000
```

---

## Application Routes 🔗

| Route         | Method | Description                   |
| ------------- | ------ | ----------------------------- |
| `/`           | GET    | Home page                     |
| `/register`   | POST   | Register new user             |
| `/login`      | GET    | Login page                    |
| `/login`      | POST   | Login user                    |
| `/profile`    | GET    | User profile (requires login) |
| `/post`       | POST   | Create a new post             |
| `/edit/:id`   | GET    | Edit post page                |
| `/update/:id` | POST   | Update post                   |
| `/like/:id`   | GET    | Like or Unlike a post         |
| `/logout`     | GET    | Logout user                   |

---

## Authentication Flow 🔐

1. User registers with email and password
2. Password is hashed using **bcrypt**
3. After login, a **JWT token** is generated
4. The token is stored in **cookies**
5. Protected routes use middleware to verify login

---

## Future Improvements 💡

* Delete posts
* Comment system
* User profile pictures
* Follow / unfollow users
* REST API version
* React frontend

---

## Author 👨‍💻

**Sampurn Samadder**
