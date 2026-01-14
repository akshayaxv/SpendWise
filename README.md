# SpendWise 💰

A comprehensive personal finance management application that helps you track expenses, manage budgets, and gain insights into your spending habits.

## Features ✨

- **Transaction Management**: Add, edit, and delete income/expense transactions
- **Receipt Scanning**: Upload and extract data from receipts using AI (Google Gemini)
- **Budget Tracking**: Set and monitor budgets for different categories
- **Recurring Transactions**: Automate regular income and expenses
- **Data Visualization**: Interactive charts and graphs for spending analysis
- **Export Data**: Download transaction history in various formats
- **Dark/Light Mode**: Comfortable viewing experience
- **Multi-Currency Support**: Track expenses in different currencies

## Tech Stack 🛠️

### Frontend
- React.js
- Tailwind CSS
- Chart.js / Recharts
- Axios

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- Google Gemini AI (for receipt scanning)

## Prerequisites 📋

Before you begin, ensure you have the following installed:
- Node.js (v14 or higher)
- MongoDB (local or MongoDB Atlas account)
- npm or yarn

## Installation 🚀

### 1. Clone the repository
```bash
git clone https://github.com/akshayaxv/SpendWise.git
cd SpendWise
```

### 2. Backend Setup

```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Create .env file
# Copy the content below and replace with your actual values
```

Create a `.env` file in the `backend` folder:
```env
PORT=5000
MONGO_URI=mongodb+srv://your-username:your-password@cluster.mongodb.net/spendwise
JWT_SECRET=your-secret-key-here
GEMINI_API_KEY=your-gemini-api-key
KEEP_ALIVE_URL=http://localhost:5000
```

**Getting API Keys:**
- **MongoDB URI**: Sign up at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) and create a cluster
- **Gemini API Key**: Get it from [Google AI Studio](https://aistudio.google.com/apikey)

```bash
# Start the backend server
npm start
```

Backend will run on `http://localhost:5000`

### 3. Frontend Setup

Open a new terminal:

```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Start the development server
npm run dev
```

Frontend will run on `http://localhost:5173`

## Usage 📖

1. **Sign Up/Login**: Create an account or login with existing credentials
2. **Add Transactions**: Manually add income or expenses
3. **Upload Receipts**: Use the receipt scanner to automatically extract transaction details
4. **Set Budgets**: Create budgets for different spending categories
5. **View Dashboard**: Analyze your spending patterns with interactive charts
6. **Manage Recurring**: Set up automatic recurring transactions

## Project Structure 📁

```
SpendWise/
├── backend/
│   ├── config/          # Database configuration
│   ├── controllers/     # Route controllers
│   ├── middleware/      # Authentication & validation middleware
│   ├── models/          # Mongoose models
│   ├── routes/          # API routes
│   ├── uploads/         # Uploaded receipt images
│   ├── server.js        # Entry point
│   └── .env             # Environment variables
├── frontend/
│   ├── public/          # Static assets
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── context/     # Context API
│   │   ├── pages/       # Page components
│   │   ├── utils/       # Utility functions
│   │   └── App.jsx      # Main app component
│   └── package.json
└── README.md
```

## API Endpoints 🔌

### Authentication
- `POST /api/auth/signup` - Register new user
- `POST /api/auth/login` - User login

### Transactions
- `GET /api/transactions` - Get all transactions
- `POST /api/transactions` - Add new transaction
- `PUT /api/transactions/:id` - Update transaction
- `DELETE /api/transactions/:id` - Delete transaction
- `GET /api/transactions/summary` - Get transaction summary
- `GET /api/transactions/charts` - Get chart data
- `GET /api/transactions/categories` - Get all categories
- `GET /api/transactions/export` - Export transactions

### Receipts
- `POST /api/receipts/upload` - Upload and process receipt

### Budgets
- `GET /api/budgets` - Get all budgets
- `POST /api/budgets` - Create budget
- `PUT /api/budgets/:id` - Update budget
- `DELETE /api/budgets/:id` - Delete budget

### Recurring Transactions
- `GET /api/recurring` - Get recurring transactions
- `POST /api/recurring` - Create recurring transaction
- `PUT /api/recurring/:id` - Update recurring transaction
- `DELETE /api/recurring/:id` - Delete recurring transaction

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author ✍️

**Akshaya V**
- GitHub: [@akshayaxv](https://github.com/akshayaxv)

## Acknowledgments 🙏

- Google Gemini AI for receipt processing
- MongoDB for database
- React community for amazing tools and libraries

## Support 💬

For support, email akshaya@example.com or open an issue in the repository.

---

Made with ❤️ by Akshaya V
