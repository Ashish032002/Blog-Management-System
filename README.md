# Blog Management System

A full-stack MERN blog platform with user authentication, post management, and real-time updates.

## Features

- User authentication with JWT
- Blog post creation and management
- Rich text editor integration
- Image upload capability
- Comment system
- Like/Unlike posts
- User roles (Admin/User)
- Responsive design

## Tech Stack

- MongoDB
- Express.js
- React
- Node.js
- Material-UI
- JWT Authentication

## Installation

### Prerequisites
- Node.js (v14+)
- MongoDB
- npm/yarn

### Backend Setup
```bash
cd server
npm install
cp .env.example .env  # Configure environment variables
npm run dev
```

### Frontend Setup
```bash
cd client
npm install
npm start
```

## Environment Variables

### Backend (.env)
```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
```

## API Documentation

### Authentication
- POST /api/auth/register - Register new user
- POST /api/auth/login - User login

### Posts
- GET /api/posts - Get all posts
- POST /api/posts - Create new post
- PUT /api/posts/:id - Update post
- DELETE /api/posts/:id - Delete post

## Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/name`)
3. Commit changes (`git commit -am 'Add feature'`)
4. Push branch (`git push origin feature/name`)
5. Create Pull Request

## License

MIT License

---

# .gitignore
```
# Dependencies
node_modules/
/.pnp
.pnp.js

# Testing
/coverage

# Production
/build
/dist

# Misc
.DS_Store
.env
.env.local
.env.development.local
.env.test.local
.env.production.local

npm-debug.log*
yarn-debug.log*
yarn-error.log*
```

# .env.example
```
MONGODB_URI=mongodb://localhost:27017/blog_db
JWT_SECRET=your_jwt_secret_here
PORT=5000
```

# .eslintrc.json
```json
{
  "env": {
    "browser": true,
    "es2021": true,
    "node": true
  },
  "extends": [
    "eslint:recommended",
    "plugin:react/recommended"
  ],
  "parserOptions": {
    "ecmaFeatures": {
      "jsx": true
    },
    "ecmaVersion": 12,
    "sourceType": "module"
  },
  "plugins": [
    "react"
  ],
  "rules": {
    "react/react-in-jsx-scope": "off",
    "react/prop-types": "off"
  }
}
```

# client/.env.example
```
REACT_APP_API_URL=http://localhost:5000/api
```

# LICENSE
```
MIT License

Copyright (c) 2024 Your Name

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
