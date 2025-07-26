# LMS - Learning Management System

A full-stack Learning Management System built with MERN stack (MongoDB, Express.js, React.js, Node.js) for instructors to create courses and students to learn.

## ✨ Features

- **Instructors**: Create courses, upload media, track enrollments
- **Students**: Browse courses, purchase with PayPal, track progress
- **Authentication**: JWT-based with role-based access
- **Payments**: PayPal integration for course purchases
- **Media**: Cloudinary integration for file uploads
- **Responsive**: Mobile-friendly design with Tailwind CSS

## 🚀 Quick Start

### Prerequisites
- Node.js (v14+)
- MongoDB
- PayPal & Cloudinary accounts

### Installation

1. **Clone & Install**
```bash
git clone <repo-url>
cd LMS-MERN
cd server && npm install
cd ../client && npm install
```

2. **Environment Setup**
Create `server/.env`:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
CLIENT_URL=http://localhost:5173
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
PAYPAL_CLIENT_ID=your_paypal_client_id
PAYPAL_SECRET_ID=your_paypal_secret_id
```

3. **Run Development Servers**
```bash
# Terminal 1 - Backend
cd server && npm run dev

# Terminal 2 - Frontend  
cd client && npm run dev
```

Visit `http://localhost:5173` to see the app!

## 🛠️ Tech Stack

**Frontend**: React, Vite, Tailwind CSS, Axios  
**Backend**: Node.js, Express, MongoDB, Mongoose  
**Services**: JWT Auth, PayPal Payments, Cloudinary Media

## 📱 API Endpoints

- `POST /auth/register` - User registration
- `POST /auth/login` - User login  
- `GET /instructor/course/*` - Course management
- `GET /student/course/*` - Course browsing
- `POST /student/order/*` - Payment processing

## 🤝 Contributing

1. Fork the repo
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details

---

⭐ Star this repo if you found it helpful! 