# Blog Application

A full-stack blogging application built with Node.js, Express, MongoDB, and EJS templates.
This repo is ready to post to GitHub and includes server code, views, environment examples, and deployment notes.

## Features
- User registration and login with session-based authentication
- Create, Read, Update, Delete blog posts (per-user)
- EJS templating for server-side rendered pages
- Basic styling and layouts
- Ready for deployment on Render/Heroku and MongoDB Atlas

## Tech Stack
- Node.js, Express.js
- MongoDB (Mongoose)
- EJS templates for views
- Express-session for session management
- Bootstrap (CDN) for basic UI

## Project structure
```
/views        -> EJS templates (layouts, pages, partials)
/public       -> static assets (CSS, images)
/models       -> Mongoose models (User, Post)
/routes       -> Express routes (auth, posts, index)
server.js
README.md
.env.example
```

## Quick start (local)

### Prerequisites
- Node.js v16+ and npm
- MongoDB URI (local or Atlas)

### Run locally
```bash
cp .env.example .env
# set MONGO_URI and SESSION_SECRET in .env
npm install
npm start
```
App runs at `http://localhost:3000` by default.

## Deployment
- Use MongoDB Atlas for the database.
- Deploy to Render/Heroku and set environment variables there.
- Ensure sessions are secured (use secure cookies and proper session store for production).

## License
MIT
