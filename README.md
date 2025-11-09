# WealthPulse 📈

> **Transforming complex finance into simple, smart decisions**

WealthPulse is a comprehensive financial technology platform that combines AI-powered insights, real-time portfolio tracking, and educational resources to help investors make smarter financial decisions across stocks, mutual funds, and cryptocurrencies.

## ✨ Features

### 🤖 AI-Powered Investment Intelligence
- **AI Investment Insights**: Get personalized recommendations powered by Google Gemini 2.0 Flash
- **Portfolio Analysis**: Comprehensive AI-driven risk assessment and trend analysis
- **Smart Chatbot**: Interactive financial assistant for instant guidance
- **Auto-Generated Reports**: Detailed portfolio reports with risk metrics and recommendations

### 📊 Real-Time Portfolio Management
- **Multi-Asset Tracking**: Stocks, mutual funds, and cryptocurrencies in one dashboard
- **Live Data Integration**: Real-time market data and price updates
- **Portfolio Analytics**: Track performance, volatility, and Sharpe ratios
- **Risk Assessment**: Automated risk categorization and volatility analysis

### 🎓 Financial Education Hub
- **Learning Courses**: Comprehensive tutorials on stocks, crypto, and mutual funds
- **Educational Content**: Videos, blogs, and interactive learning materials
- **Beginner-Friendly**: Designed to grow your financial literacy step by step

### 🔐 Secure Authentication
- **Auth0 Integration**: Enterprise-grade authentication and user management
- **Personalized Experience**: User-specific portfolios and preferences
- **Secure Data**: Protected user financial information

## 🛠️ Tech Stack

### Frontend
- **Next.js 15.5.3** with App Router
- **React 19.1.0** with modern hooks
- **TypeScript** for type safety
- **Tailwind CSS 4.1.16** for styling
- **Framer Motion** for animations
- **Recharts** for data visualization

### Backend
- **FastAPI** Python backend
- **MongoDB** for data persistence
- **Auth0** for authentication
- **OpenRouter API** with Google Gemini 2.0

### Key Dependencies
- `@auth0/nextjs-auth0` - Authentication
- `openai` - AI model integration via OpenRouter
- `axios` - HTTP client
- `recharts` - Charts and graphs
- `framer-motion` - Animations
- `lucide-react` - Icons

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- Python 3.8+
- MongoDB instance
- OpenRouter API key
- Auth0 account

### Environment Variables

Create a `.env.local` file in the root directory:

```env
# Auth0 Configuration
AUTH0_SECRET=your_auth0_secret
AUTH0_BASE_URL=http://localhost:3000
AUTH0_ISSUER_BASE_URL=https://your-domain.auth0.com
AUTH0_CLIENT_ID=your_client_id
AUTH0_CLIENT_SECRET=your_client_secret

# OpenRouter AI
OPENROUTER_API_KEY=your_openrouter_api_key

# MongoDB
MONGODB_URI=your_mongodb_connection_string
```

### Frontend Setup

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

### Backend Setup

```bash
# Navigate to backend directory
cd backend

# Install Python dependencies
pip install -r requirements.txt

# Run FastAPI server
python main.py
```

Open [http://localhost:3000](http://localhost:3000) to view the application.

## 📁 Project Structure

```
wealthpulse/
├── app/                          # Next.js App Router
│   ├── components/              # React components
│   │   ├── Navbar.jsx
│   │   ├── Hero.jsx
│   │   ├── Chatbot.jsx
│   │   └── ...
│   ├── api/                     # API routes
│   │   ├── ai/                  # AI-powered endpoints
│   │   ├── auth/                # Authentication
│   │   ├── portfolio/           # Portfolio management
│   │   └── chat/                # Chatbot API
│   ├── StockDashboard/          # Stock tracking pages
│   ├── CryptoDashboard/         # Crypto tracking pages
│   ├── MFDashboard/            # Mutual fund pages
│   ├── Portfolio/               # Portfolio management
│   └── Courses/                 # Educational content
├── backend/                     # FastAPI backend
│   ├── main.py                  # FastAPI application
│   ├── stock_api.py            # Stock data API
│   ├── crypto_api.py           # Crypto data API
│   ├── mf_api.py               # Mutual fund API
│   └── portfolio_mongodb.py    # Portfolio management
├── components/                  # Shared UI components
├── lib/                        # Utility functions
└── public/                     # Static assets
```

## 🔗 API Endpoints

### AI Services
- `POST /api/ai/generate-report` - Generate AI portfolio reports
- `POST /api/ai/summarize` - Summarize financial data
- `POST /api/chat` - Chatbot interactions

### Portfolio Management
- `GET /api/portfolio/[userId]` - Get user portfolio
- `POST /api/portfolio/add/[userId]` - Add portfolio item
- `PUT /api/portfolio/[userId]/[itemId]` - Update portfolio item

### Authentication
- `/api/auth/[auth0]` - Auth0 authentication endpoints

## 🎯 Key Features in Detail

### AI-Powered Analysis
WealthPulse leverages Google Gemini 2.0 Flash through OpenRouter to provide:
- Risk assessment and volatility analysis
- Personalized investment recommendations
- Market trend analysis
- Portfolio optimization suggestions

### Multi-Asset Support
Track and analyze:
- **Stocks**: Real-time prices, technical indicators
- **Mutual Funds**: NAV tracking, fund performance
- **Cryptocurrencies**: Price movements, market cap

### Educational Platform
- Interactive courses on financial literacy
- Video tutorials and guides
- Blog content on investment strategies
- Beginner to advanced learning paths

## 🔧 Available Scripts

```bash
npm run dev      # Start development server with Turbopack
npm run build    # Build for production with Turbopack
npm run start    # Start production server
npm run lint     # Run ESLint
```

## 🚀 Deployment

### Vercel (Recommended)
1. Connect your GitHub repository to Vercel
2. Configure environment variables
3. Deploy with automatic CI/CD

### Manual Deployment
1. Build the application: `npm run build`
2. Deploy the `.next` folder to your hosting provider
3. Set up the FastAPI backend on your preferred cloud platform

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📄 License

This project is private and proprietary.

## 🆘 Support

For support and questions:
- Open an issue on GitHub
- Contact the development team
- Check the documentation in `/docs`

---

Built with ❤️ using Next.js, FastAPI, and AI technology to democratize financial intelligence.
