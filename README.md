# 📊 InsightBoard – Admin Analytics Dashboard

InsightBoard is a modern, full-stack Admin Analytics Dashboard designed to manage business operations and monitor important business metrics through a clean and interactive interface.

It provides customer management, product management, order tracking, business analytics, and secure authentication with role-based access control.

## 🚀 Features

### 📈 Dashboard & Analytics
- Business overview with key performance indicators.
- Total revenue, orders, customers, and products.
- Revenue and order analytics.
- Order status distribution.
- Date-based analytics and custom date ranges.
- Interactive charts and visualizations.

### 👥 Customer Management
- View customer records.
- Add, update, and delete customers.
- Search and filter customers.
- Customer status management.
- Pagination and sorting.

### 📦 Product Management
- Add and manage products.
- Update product information.
- Delete products.
- Search and filter products.
- Track product prices and stock.
- Product status management.

### 🛒 Order Management
- Create and manage orders.
- Update order information.
- Track order status.
- Search and filter orders.
- Monitor order details and revenue.

### 🔐 Authentication & Security
- Secure login and registration.
- Google authentication.
- JWT-based authentication.
- Password hashing using bcrypt.
- Role-based access control.
- Separate Admin and Viewer permissions.

## 🛠️ Technology Stack

### Frontend
- React.js
- Vite
- JavaScript
- CSS
- React Router
- Axios
- Recharts
- Lucide React
- TanStack React Table

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Token (JWT)
- bcryptjs
- Google OAuth

## 📁 Project Structure

```text
InsightBoard/
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── scripts/
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── services/
│   │   └── styles/
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/anushkasingh1603/InsightBoard.git
```

Navigate to the project directory:

```bash
cd InsightBoard
```

### 2. Setup Backend

Navigate to the backend folder:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the backend folder:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
ADMIN_NAME=your_admin_name
ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_secure_password
GOOGLE_CLIENT_ID=your_google_client_id
```

Start the backend server:

```bash
npm run dev
```

Backend will run at:

```text
http://localhost:5000
```

### 3. Setup Frontend

Open another terminal and navigate to the frontend folder:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the frontend folder:

```env
VITE_API_URL=http://localhost:5000/api
VITE_GOOGLE_CLIENT_ID=your_google_client_id
```

Start the frontend:

```bash
npm run dev
```

Frontend will run at the local Vite development URL displayed in your terminal (usually `http://localhost:5173`).

## 🔑 Environment Variables

| Variable | Description |
|---|---|
| PORT | Backend server port |
| MONGO_URI | MongoDB database connection |
| JWT_SECRET | Secret key for JWT authentication |
| ADMIN_NAME | Default administrator name |
| ADMIN_EMAIL | Default administrator email |
| ADMIN_PASSWORD | Default administrator password |
| GOOGLE_CLIENT_ID | Google OAuth client ID |
| VITE_API_URL | Backend API URL for frontend |
| VITE_GOOGLE_CLIENT_ID | Google OAuth client ID for frontend |

**Important:** Never upload `.env` files, passwords, database credentials, or secret keys to GitHub.

## 🌐 API Routes

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/login` | User login |
| POST | `/api/auth/register` | User registration |
| POST | `/api/auth/google` | Google authentication |
| GET | `/api/dashboard` | Dashboard analytics |
| GET | `/api/customers` | Fetch customers |
| GET | `/api/products` | Fetch products |
| GET |
