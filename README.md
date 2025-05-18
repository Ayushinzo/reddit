# Reddit Clone

A full-stack Reddit clone built with Next.js 13, Express.js, and MongoDB. Features user authentication, community creation, post management, and real-time interactions.

![Reddit Clone](public/reddit.png)

## 🌟 Features

- **User Authentication** with Clerk.js
- **Community Management**
  - Create and join communities
  - Custom community avatars
  - Community descriptions and rules
- **Post Management**
  - Create posts with text, images, and videos
  - Rich text formatting
  - Media upload support
- **Interactive Features**
  - Upvote/downvote posts
  - Comment on posts
  - Share posts
- **Real-time Updates**
- **Responsive Design**
- **Trending & Recent Posts**

## 🛠️ Tech Stack

### Frontend
- **Framework**: Next.js 13 (App Router)
- **Styling**: Tailwind CSS
- **Authentication**: Clerk.js
- **State Management**: React Context
- **HTTP Client**: Axios
- **Icons**: React Icons
- **UI Components**: Custom components
- **Form Handling**: Express Validator

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB
- **ODM**: Mongoose
- **File Upload**: Multer
- **Cloud Storage**: Cloudinary
- **Validation**: Express Validator
- **Development**: Nodemon

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- MongoDB
- npm or yarn
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/reddit-clone.git
cd reddit-clone
```

2. Install frontend dependencies:
```bash
cd frontend
npm install
```

3. Install backend dependencies:
```bash
cd ../backend
npm install
```

### Environment Setup

1. Frontend Environment (.env.local):
```env
NEXT_PUBLIC_BACKEND_URL=http://localhost:5000
NEXT_PUBLIC_WEBSITE_URL=http://localhost:3000
NEXT_PUBLIC_CLERK_SIGN_IN_FALLBACK_REDIRECT_URL=/home
NEXT_PUBLIC_CLERK_SIGN_UP_FALLBACK_REDIRECT_URL=/home
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=clerk_api_key
CLERK_SECRET_KEY=clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
```

2. Backend Environment (.env):
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

### Running the Application

1. Start the backend server:
```bash
cd backend
npm run server
```

2. Start the frontend development server:
```bash
cd frontend
npm run dev
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser

## 📁 Project Structure

```
reddit-clone/
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   │   ├── (components)/
│   │   │   ├── home/
│   │   │   └── layout.js
│   │   └── functions.js
│   ├── public/
│   └── package.json
└── backend/
    ├── routes/
    ├── models/
    ├── cloudinary/
    ├── connectdb/
    ├── multer/
    └── index.js
```

## 🔑 Key Features Implementation

### User Authentication
- Secure authentication using Clerk.js
- Protected routes and API endpoints
- User profile management

### Post Management
- Create, read, update, and delete posts
- Media upload support (images and videos)
- Voting system
- Comment threading

### Community Features
- Create and manage communities
- Join/leave communities
- Community-specific posts
- Custom community settings

## 🤝 Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

Your Name - [@yourusername](https://github.com/yourusername)

## 🙏 Acknowledgments

- Next.js team for the amazing framework
- Clerk.js for authentication
- MongoDB for the database
- Cloudinary for media storage