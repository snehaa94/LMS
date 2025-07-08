# 📚 Full-Stack Learning Management System (LMS)

A fully-featured **Learning Management System (LMS)** built with the **MERN stack** (MongoDB, Express.js, React.js, Node.js). This platform allows **instructors** to create and manage courses and enables **students** to browse, enroll, and access content with an integrated **Stripe payment system**.

---

## ✨ Key Features

### 🧑‍🏫 Admin / Instructor Capabilities

- ✅ Add, update, or delete courses
- 🎓 Manage course content:
  - Course Title, Subtitle, and Description
  - Course Category & Level (Beginner, Intermediate, Advanced)
  - Pricing & Estimated Pricing
  - Course Thumbnail Upload via **Cloudinary**
- 📤 Publish or Unpublish Courses
- 🖼️ Dashboard with Course Statistics
- 🔐 Protected admin routes using JWT & Role-based access

---

### 🎓 Student Capabilities

- 🔍 Browse all available courses
- 📖 View detailed course information
- 💳 Enroll in paid courses via **Stripe**
- 🔓 Access content after successful enrollment
- 📚 View My Courses section with enrolled content
- 👤 Update Profile Info & Avatar

---

## 💳 Stripe Payment Integration

Secure and seamless integration with **Stripe** for handling course payments.

### Payment Flow:

- Course enrollment is initiated via Stripe Checkout
- On successful payment, the course is auto-added to the student's account
- Backend verifies transactions securely before granting access

### ✅ Completed Stripe Features:

- Secure Stripe Checkout Sessions
- Payment confirmation handling
- Automatic course access post-payment

### 🔜 Upcoming Stripe Features:

- 🧾 View payment history
- 📧 Email invoices and confirmations
- 🏷️ Discount coupon system
- 🔁 Subscription-based course access

---

## 🔐 Authentication & Authorization

- JWT-based authentication
- Role-based access control (Admin / Instructor / Student)
- Secure cookies for session persistence
- Route protection (Frontend & Backend)

---

## 🛠️ Tech Stack

| Layer          | Tech Used                                    |
|----------------|----------------------------------------------|
| Frontend       | React.js, Tailwind CSS, ShadCN UI             |
| State Mgmt     | Redux Toolkit + RTK Query                     |
| Backend        | Node.js, Express.js                          |
| Database       | MongoDB with Mongoose                        |
| Media Uploads  | Cloudinary (Course Thumbnails, Avatars)      |
| File Uploads   | Multer                                       |
| Authentication | JWT + Cookies                                |
| Payment        | Stripe                                       |

---

## 📦 Project Structure

```
LMS/
├── client/        # React Frontend
├── server/        # Node/Express Backend
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middlewares/
│   ├── utils/
│   └── config/
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/snehaa94/LMS.git
cd LMS
```

### 2. Install Dependencies

```bash
# Frontend
cd client
npm install

# Backend
cd ../server
npm install
```

### 3. Create Environment File

Create a `.env` file inside the `server` directory:

```env
PORT=8080
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_KEY=your_cloudinary_key
CLOUDINARY_SECRET=your_cloudinary_secret
STRIPE_SECRET_KEY=your_stripe_secret
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
```

### 4. Start the App

```bash
# Start Backend
cd server
npm run dev

# Start Frontend
cd ../client
npm run dev
```

---

## 📸 Demo Screenshots

![auth](https://github.com/user-attachments/assets/05fdcc14-a073-4924-a61b-6677f66e30eb)

![home](https://github.com/user-attachments/assets/d53bd216-9b77-4d7a-b3d7-30ee8c037f53)

![edit](https://github.com/user-attachments/assets/5b9990fe-679f-48cb-ac3f-781ec4e5cec7)

![course](https://github.com/user-attachments/assets/4499a177-19e9-4396-bd6c-6b2933b0444e)

![courseEdit](https://github.com/user-attachments/assets/08ddc021-fa18-47ee-aa30-41bd22f71e17)

![dashboard](https://github.com/user-attachments/assets/b0352409-9295-4dc7-ab2e-94b5c4eadeed)

![Screenshot (43)](https://github.com/user-attachments/assets/7189c5ba-7dec-48f0-9dfa-2d188a7ff3be)

![Screenshot (44)](https://github.com/user-attachments/assets/d6c06063-5b79-44d8-8891-d5014987fb4e)

---

## 🧪 Stripe Test Card Details

Use the following test card for Stripe payments during development:

```
Card Number: 4242 4242 4242 4242
Exp Date: Any future date (MM/YY)
CVC: Any 3-digit number (e.g., 123)
ZIP: Any 5-digit number (e.g., 12345)
```

> ⚠️ Ensure you’re using **Stripe Test Keys** to avoid real transactions.

---

## 📫 Feedback and Contributions

- Fork this repo and feel free to raise PRs
- Open issues for suggestions or bugs
- Star ⭐ the project if you find it useful!

---

## 👩‍💻 Author

**Sneha Kashyap**  
[GitHub Profile](https://github.com/snehaa94)

---

## 📄 License

This project is licensed under the **MIT License**.

---
