# AVONE - E-commerce Platform

## 🚀 Overview
ECOM1 is a full-stack e-commerce platform that enables users to browse, add to cart, and purchase products. It includes authentication, order management, and payment processing.

## 📂 Project Structure
```
ECOM1/
│── client/      # Frontend (React.js, Next.js)
│── server/      # Backend (Node.js, Express, Prisma)
│── prisma/      # Database schema and migrations
│── .gitignore   # Git ignore file
│── docker-compose.yml  # Docker setup
│── README.md    # Project documentation
```

## 🛠️ Tech Stack
### **Frontend:**
- React.js (Next.js)
- TypeScript
- TailwindCSS
- ShadCN components (with react-hot-toast for notifications)

### **Backend:**
- Node.js (Express.js)
- Prisma ORM (PostgreSQL)
- Cloudinary (for image uploads)
- Authentication (JWT, bcrypt)

### **Payments & Notifications:**
- PayPal Sandbox Integration
- React-Hot-Toast for alerts

## 🚀 Installation & Setup

### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/Harshu1121/ECOM1.git
cd ECOM1
```

### **2️⃣ Install Dependencies**
#### **Backend**
```sh
cd server
npm install
```

#### **Frontend**
```sh
cd ../client
npm install
```

### **3️⃣ Set Up Environment Variables**
Create a `.env` file in the **server** directory and add:
```env
DATABASE_URL=your_database_url
JWT_SECRET=your_jwt_secret
CLOUDINARY_URL=your_cloudinary_url
PAYPAL_CLIENT_ID=your_paypal_client_id
PAYPAL_CLIENT_SECRET=your_paypal_client_secret
```

### **4️⃣ Run Database Migrations**
```sh
npx prisma migrate dev
```

### **5️⃣ Start the Backend**
```sh
cd server
npm run dev
```

### **6️⃣ Start the Frontend**
```sh
cd client
npm run dev
```

## 🎯 Features
- 🛒 Product Management (Add, Update, Delete Products)
- 🔒 User Authentication (Register, Login, JWT-based Auth)
- 📦 Order & Cart Management
- 💳 PayPal Payment Integration
- 📢 Toast Notifications (Success/Error messages with react-hot-toast)
- 📷 Image Uploads with Cloudinary

## 📜 Usage
- Visit `http://localhost:3000` for frontend.
- API runs on `http://localhost:5000`.
- To test PayPal sandbox, use test accounts from the PayPal Developer portal.

## 🛠️ Deployment
For production, set up the environment variables and use:
```sh
npm run build
npm start
```

## 🤝 Contribution
1. Fork the repo.
2. Create a new branch: `git checkout -b feature-branch`
3. Commit your changes: `git commit -m "Added feature X"`
4. Push to the branch: `git push origin feature-branch`
5. Open a Pull Request.

## 📜 License
This project is licensed under the MIT License.

