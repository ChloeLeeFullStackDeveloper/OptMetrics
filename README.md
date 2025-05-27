# OptMetrics - Optometry Practice Management System

## 🎯 Project Overview

OptMetrics is a comprehensive web-based practice management system designed specifically for optometry clinics. This full-stack application demonstrates modern web development skills, business intelligence capabilities, and database management - showcasing the complete skill set required for BI & Web Developer positions.

## 🚀 Live Demo

- **Frontend:** [Live Application](https://optmetrics.vercel.app) *(Deploy link will be added)*
- **API Documentation:** [API Docs](https://optmetrics-api.railway.app/docs) *(Deploy link will be added)*
- **Power BI Dashboard:** [Analytics Dashboard](link-to-powerbi) *(Will be embedded)*

## 📋 Features

### Core Functionality
- **Patient Management** - Complete CRUD operations for patient records
- **Appointment Scheduling** - Interactive calendar with booking system
- **User Authentication** - Role-based access (Admin, Doctor, Staff)
- **Business Intelligence Dashboard** - Real-time analytics and KPIs
- **Reporting System** - Exportable reports in CSV/PDF formats
- **CRM Features** - Patient communication logs and follow-up tracking

### Technical Highlights
- **Responsive Design** - Mobile-first approach with CSS Grid/Flexbox
- **Real-time Updates** - Live data synchronization across users
- **Data Visualization** - Interactive charts and graphs
- **Power BI Integration** - Embedded analytics dashboard
- **RESTful API** - Clean, documented API endpoints
- **Security** - JWT authentication, input validation, SQL injection protection

## 🛠️ Technology Stack

### Frontend
- **React 18** - Component-based UI framework
- **React Router** - Client-side routing
- **Recharts** - Data visualization library
- **CSS Modules** - Scoped styling
- **Axios** - HTTP client for API calls

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web application framework
- **PostgreSQL** - Relational database
- **JWT** - Authentication tokens
- **bcryptjs** - Password hashing
- **cors** - Cross-origin resource sharing

### DevOps & Tools
- **Vercel** - Frontend deployment
- **Railway** - Backend and database hosting
- **Git/GitHub** - Version control
- **Postman** - API testing
- **Power BI** - Business intelligence platform

## 📊 Business Intelligence Features

### Analytics Dashboard
- **Patient Demographics** - Age distribution, insurance types, geographic data
- **Appointment Trends** - Monthly/weekly patterns, peak hours analysis
- **Revenue Tracking** - Procedure profitability, payment method analysis
- **Operational KPIs** - Wait times, appointment completion rates
- **Growth Metrics** - New vs returning patients, retention rates

### Reporting Capabilities
- **Financial Reports** - Revenue summaries, outstanding payments
- **Patient Reports** - Visit history, treatment tracking
- **Operational Reports** - Staff productivity, equipment utilization
- **Export Options** - CSV, PDF, Excel formats
- **Scheduled Reports** - Automated daily/weekly/monthly reports

## 🏗️ System Architecture

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   React App     │    │   Express API   │    │   PostgreSQL    │
│   (Frontend)    │◄──►│   (Backend)     │◄──►│   Database      │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│     Vercel      │    │    Railway      │    │   Power BI      │
│   (Hosting)     │    │   (Hosting)     │    │  (Analytics)    │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

## 📦 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- PostgreSQL (v12 or higher)
- Git

### Local Development Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/optmetrics.git
   cd optmetrics
   ```

2. **Backend Setup**
   ```bash
   cd backend
   npm install
   
   # Create .env file
   cp .env.example .env
   # Edit .env with your database credentials
   
   # Run database migrations
   npm run migrate
   
   # Seed sample data
   npm run seed
   
   # Start development server
   npm run dev
   ```

3. **Frontend Setup**
   ```bash
   cd frontend
   npm install
   
   # Create .env file
   cp .env.example .env
   # Edit .env with API URL
   
   # Start development server
   npm start
   ```

4. **Access the application**
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000`
   - API Documentation: `http://localhost:5000/docs`

### Environment Variables

#### Backend (.env)
```env
PORT=5000
DATABASE_URL=postgresql://username:password@localhost:5432/optmetrics
JWT_SECRET=your_jwt_secret_key
NODE_ENV=development
```

#### Frontend (.env)
```env
REACT_APP_API_URL=http://localhost:5000
REACT_APP_POWERBI_EMBED_URL=your_powerbi_url
```

## 📚 API Documentation

### Authentication Endpoints
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `POST /api/auth/refresh` - Refresh JWT token

### Patient Management
- `GET /api/patients` - Get all patients
- `GET /api/patients/:id` - Get patient by ID
- `POST /api/patients` - Create new patient
- `PUT /api/patients/:id` - Update patient
- `DELETE /api/patients/:id` - Delete patient

### Appointment Management
- `GET /api/appointments` - Get all appointments
- `GET /api/appointments/date/:date` - Get appointments by date
- `POST /api/appointments` - Create appointment
- `PUT /api/appointments/:id` - Update appointment
- `DELETE /api/appointments/:id` - Cancel appointment

### Analytics & Reports
- `GET /api/analytics/dashboard` - Dashboard KPIs
- `GET /api/analytics/patients/demographics` - Patient demographics
- `GET /api/analytics/revenue/monthly` - Monthly revenue data
- `GET /api/reports/export/:type` - Export reports (CSV/PDF)

## 🧪 Testing

### Running Tests
```bash
# Backend tests
cd backend
npm test

# Frontend tests
cd frontend
npm test

# End-to-end tests
npm run test:e2e
```

### Test Coverage
- Unit tests for all API endpoints
- Component testing for React components
- Integration tests for database operations
- End-to-end testing for critical user flows

## 🚀 Deployment

### Frontend (Vercel)
1. Connect GitHub repository to Vercel
2. Set environment variables in Vercel dashboard
3. Deploy automatically on push to main branch

### Backend (Railway)
1. Connect GitHub repository to Railway
2. Add PostgreSQL database service
3. Set environment variables
4. Deploy automatically on push to main branch

## 📈 Performance Optimization

- **Code splitting** - Lazy loading of React components
- **Image optimization** - Compressed and responsive images
- **Database indexing** - Optimized queries for large datasets
- **Caching** - Redis for frequently accessed data
- **CDN** - Static asset delivery via Vercel Edge Network

## 🔒 Security Features

- **Authentication** - JWT-based secure authentication
- **Authorization** - Role-based access control
- **Input Validation** - Server-side validation for all inputs
- **SQL Injection Protection** - Parameterized queries
- **HTTPS** - SSL/TLS encryption in production
- **Rate Limiting** - API endpoint protection

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 👨‍💻 Developer

**Your Name**
- Portfolio: [your-portfolio.com](https://your-portfolio.com)
- LinkedIn: [linkedin.com/in/yourprofile](https://linkedin.com/in/yourprofile)
- Email: your.email@example.com

## 🙏 Acknowledgments

- Built as a portfolio project demonstrating full-stack development skills
- Designed to showcase business intelligence and web development capabilities
- Created for optometry professionals to streamline practice management

---

*This project demonstrates proficiency in React, Node.js, PostgreSQL, business intelligence, and modern web development practices - perfect for BI & Web Developer positions.*