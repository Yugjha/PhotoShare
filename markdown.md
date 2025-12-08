# PhotoShare – Image Album Web App

PhotoShare is a full-stack web application that allows users to log in with Google, create albums, upload images to Cloudinary, preview them in full resolution, mark favourites, and track storage usage. All data is stored securely in MongoDB.  
It is built using the MERN stack with a clean, fast, and scalable architecture.

---

🔗 **Live Demo:**
[PhotoStore]()

---

🗂 **GitHub Repositories:**

[PhotoStore]()

---

## Login (Demo Credentials)

> **Guest**
> Username: `your google account`

---

## Tech Stack

- **Frontend**: React.js
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: Google OAuth 2.0, JSON Web Token
- **Image Storage**: Cloudinary

---

## Key Features

### 1. Dashboard

- Displays user information: **name, email, profile photo**
- Shows:
  - Total albums
  - Total images
  - Total favourite images
  - Storage used

---

### 2. Album Management

- Create unlimited albums
- View all user albums
- Delete albums
- Each album has a unique ID

---

### 3. Image Uploading

- Upload multiple images at once
- Images stored automatically in Cloudinary
- Metadata stored in MongoDB
- Each image stores:
  - Image title
  - Tags
  - File size
  - Uploaded date

---

### 4. Image Preview

- View image in high resolution
- Zoom and inspect details
- See metadata in sidebar
- Navigate between album images

---

### 5. Favourites Feature

- Mark or unmark any image as favourite
- Favourite images shown on a separate page
- Dashboard shows favourite count

---

### 6. Storage Tracking

- Real-time calculation of total storage used
- Displayed visually on dashboard

---

### 7. Secure Authentication

- Login using **Google OAuth 2.0**
- Backend verifies Google token
- JWT generated for secure sessions
- Tokens stored using httpOnly cookies

---

### 8. Fully Responsive UI

- Built with React + Tailwind CSS
- Works on all screen sizes (mobile, tablet, desktop)

---

## Project Structure

PhotoShare/
│
├── backend/
│ ├── controllers/
│ ├── models/
│ ├── routers/
│ ├── middlewares/
│ ├── config/
│ ├── index.js
│ └── .env
│
└── frontend/
├── src/
│ ├── api/
│ ├── components/
│ ├── context/
│ ├── pages/
│ ├── message/
│ ├── routes/
│ ├── utils/
│ └── App.jsx

## 🌐 Project Setup

To set up and run this project locally:

1.  **Clone the Repository**:

    ```bash
    git clone
    cd frontend
    ```

2.  **Install Dependencies**:

    ```bash
    cd backend
    npm install
    ```

3.  **Environment Variables**:

    - Create a `.env` file in the root directory and add the following:

      ```env
      MONGO_URI=your_mongodb_connection_string
      JWT_TOKEN=your_jwt_secret
      PORT=9500
      NODE_ENV=development
      CLOUDINARY_API_KEY=your cloudinary api key
      CLOUDINARY_API_SECRET=your cloudinary api secret
      CLOUDINARY_CLOUD_NAME=your api cloud name
      GOOGLE_CLIENT_ID=your google client id
      GOOGLE_CLIENT_SECRET=your google client secret
      GOOGLE_REDIRECT_URI=http://localhost:5173 | redirect google url
      ```

4.  **Run the Application**:
    ```bash
    npm run dev
    ```

## 🤝 Contributing

We welcome contributions! Please feel free to submit issues, fork the repository, and open pull requests.

## 🌟 Acknowledgements

- Thanks to the developers and contributors of MongoDB, Express.js, React.js, Node.js, Stripe, and Razorpay for their fantastic tools and libraries.

---

## 🧩 Backend API Endpoints Example

1. GET /api/v1/google - GET user login via Google

```
{
  "success": true,
  "message": "Account Created Successfully" || "Logged In Successfully",
  "data":
    {
      "_id": "64f1e2a2b12c3d4567890abc",
      "name": "sushant singh"
      "email": "sushants2711@gmail.com",
      "profile_pic": "profile pic url"
    }
}

```

## Contact

For bugs or feature request, please reach out to sushants2711@gmail.com

[Linkedin](https://www.linkedin.com/in/sushant-kumar-singh-414782230)
