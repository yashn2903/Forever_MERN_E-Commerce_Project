
# FOREVER (MERN E-Commerce project)

FOREVER is a clothing e-commerce platform built on the MERN stack (MongoDB, Express, React, Node.js). It features secure payments with Razorpay & Stripe, image storage via Cloudinary, and a modern, responsive UI. Designed for scalability, it delivers a seamless online shopping experience for fashion enthusiasts.

![ecommerce-banner]()
## Project Setup

**Prerequisites**

- Node.js
- Mongodb Atlas
- Cloudinary

### Install dependencies for frontend and backend separately

**Frontend:**
```bash
  npm install

  npm install react-router-dom react-toastify
```

**Backend:**
```bash
  npm install

  npm i cors dotenv express jsonwebtoken mongoose multer nodemon razorpay stripe validator cloudinary bcrypt 
```

**Admin:**
```bash
  npm install

  npm install axios react-router-dom react-toastify
```
## Environment Variables

**Backend**
- Create a `.env` file in the `backend` directory.
- Add the following variables with appropriate values

```bash

JWT_SECRET = "-------- Anything --------"
ADMIN_EMAIL = "admin@example.com"
ADMIN_PASSWORD = "admin123"

MONGODB_URI = "-------- Paste Your Mongo URI Here --------"

CLOUDINARY_API_KEY = "-------- Paste Cloudinary API key --------"
CLOUDINARY_SECRET_KEY = "-------- Paste Cloudinary SECRET key --------"
CLOUDINARY_NAME = "-------- Paste Cloudinary cloud name --------"

STRIPE_SECRET_KEY = "-------- Paste Stripe Secret key --------"

RAZORPAY_KEY_SECRET = '-------- Paste Razorpay Secret key --------'
RAZORPAY_KEY_ID = '-------- Paste Razorpay key Id --------'


```

**Frontend**
- Create a `.env` file in the `frontend` directory
- Add the following variable:
```bash

VITE_BACKEND_URL = "http://localhost:4000"
VITE_RAZORPAY_KEY_ID = '-------- Paste Razorpay key Id --------'

```

**Admin**
- Create a `.env` file in the `admin` directory
- Add the following variable:
```bash

VITE_BACKEND_URL = "http://localhost:4000"

```

## Running Development Servers

#### Start the backend server:
- Navigate to the `backend` directory: `cd backend`
- Start the server: `npm run server`
     
#### Start the frontend server:
- Navigate to the `frontend` & `admin` directory: `cd frontend`  / `cd admin`
- Start the server: `npm run dev`