# Synchrony Training Hub

A cutting-edge React application designed for Synchrony Bank's global agent training program. This enterprise-grade platform provides real-time empathy training, performance analytics, and AI-powered coaching for customer service agents worldwide.

## 🏆 Features

### 🚀 Core Capabilities
- **Real-time Empathy Training**: Live conversation simulation with AI-powered empathy scoring
- **Performance Analytics**: Comprehensive dashboards with charts and insights
- **Agent Management**: Complete agent profiles with skill assessments and progress tracking
- **Smart API Integration**: Seamless connection to AWS Lambda endpoints with intelligent fallbacks
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices

### 🎨 Design Excellence
- **Synchrony Branding**: Official Synchrony colors (#003DA5 blue, #FFD100 yellow)
- **Material-UI Components**: Professional, accessible, and consistent UI elements
- **Smooth Animations**: Framer Motion animations for enhanced user experience
- **Modern Gradients**: Beautiful gradients and hover effects throughout

### 📊 Analytics & Insights
- **Real-time Metrics**: Live performance indicators and session tracking
- **Data Visualization**: Interactive charts using Recharts library
- **Trend Analysis**: Weekly performance trends and improvement tracking
- **Scenario Performance**: Detailed analysis of training scenario effectiveness

## 🛠️ Technology Stack

- **React 18.2.0**: Modern functional components with hooks
- **Material-UI 5.14.17**: Enterprise-grade component library
- **Framer Motion 10.16.4**: Professional animations and transitions
- **React Router 6.18.0**: Client-side routing for SPA navigation
- **Recharts 2.8.0**: Beautiful and responsive data visualization
- **Axios 1.6.0**: HTTP client for API communication
- **Context API**: Global state management for scalable architecture

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ installed
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd synchrony-training-hub
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm start
   ```

4. **Open in browser**
   ```
   http://localhost:3000
   ```

### Build for Production

```bash
npm run build
```

This creates a `build` folder with optimized production files ready for deployment.

## 🌐 Deployment

### Vercel (Recommended)

1. **Install Vercel CLI**
   ```bash
   npm i -g vercel
   ```

2. **Deploy to Vercel**
   ```bash
   vercel --prod
   ```

3. **Access your deployed app**
   Your app will be available at: `https://your-app-name.vercel.app`

### Alternative Deployment Options

- **Netlify**: Drag and drop the `build` folder to Netlify
- **AWS S3 + CloudFront**: Upload build files to S3 bucket with CloudFront distribution
- **Azure Static Web Apps**: Connect GitHub repository for automatic deployments

## 🔧 Configuration

### API Endpoints

The application is configured to work with the following AWS Lambda endpoints:

```javascript
// src/services/apiService.js
const API_BASE_URL = 'https://your-api-gateway-url.amazonaws.com/dev';

const endpoints = {
  startScenario: '/start-scenario',
  sendMessage: '/send-message', 
  getAnalysis: '/get-analysis'
};
```

### Environment Variables

Create a `.env` file in the root directory:

```env
REACT_APP_API_BASE_URL=https://your-api-gateway-url.amazonaws.com/dev
REACT_APP_ENVIRONMENT=production
```

## 📱 Application Structure

```
src/
├── components/
│   └── Layout/
│       ├── Header.js          # Navigation header with branding
│       └── Sidebar.js         # Collapsible navigation sidebar
├── context/
│   └── AppContext.js          # Global state management
├── pages/
│   ├── Welcome.js             # Landing page with feature overview
│   ├── Dashboard.js           # Agent management dashboard
│   ├── AgentProfile.js        # Detailed agent profile view
│   ├── TrainingSession.js     # Live training interface
│   └── Analytics.js           # Performance analytics dashboard
├── services/
│   └── apiService.js          # API integration layer
├── App.js                     # Main application component
├── App.css                    # Global styles and animations
└── index.js                   # Application entry point
```

## 🎯 Key Features Walkthrough

### 1. Welcome Page
- Hero section with animated statistics
- Feature showcase with icons and descriptions
- Active agent preview cards
- Call-to-action for getting started

### 2. Dashboard
- Agent grid with search and filtering
- Status-based tabs (All, Available, Training, In Session)
- Quick actions for starting training sessions
- Real-time status updates

### 3. Agent Profile
- Comprehensive agent information
- Performance charts and analytics
- Contact details and skill assessments
- Session history and progress tracking

### 4. Training Session
- Real-time conversation interface
- Live empathy scoring with AI feedback
- Response time analysis
- Session progress tracking

### 5. Analytics
- Multiple dashboard views with tabs
- Interactive charts and visualizations
- Agent rankings and performance comparisons
- Department insights and scenario analysis

## 🎨 Design System

### Colors
- **Primary Blue**: #003DA5 (Synchrony brand blue)
- **Secondary Yellow**: #FFD100 (Synchrony brand yellow)
- **Success Green**: #28a745
- **Warning Orange**: #fd7e14
- **Danger Red**: #dc3545
- **Text Gray**: #6c757d

### Typography
- **Headers**: Roboto font family, bold weights
- **Body text**: Clean, readable typography with proper spacing
- **Interactive elements**: Clear hierarchy and visual feedback

### Animations
- **Page transitions**: Smooth fade and slide animations
- **Hover effects**: Subtle elevation and color changes
- **Loading states**: Professional skeleton loaders
- **Micro-interactions**: Button clicks, form submissions

## 🔐 Security Features

- **Input validation**: All user inputs are validated and sanitized
- **Error boundaries**: Graceful error handling throughout the application
- **Fallback mechanisms**: Intelligent fallbacks when APIs are unavailable
- **Responsive design**: Works securely across all device types

## 📈 Performance Optimizations

- **Code splitting**: Lazy loading for optimal bundle sizes
- **Image optimization**: Responsive images with proper compression
- **Caching strategies**: Efficient API response caching
- **Bundle analysis**: Optimized webpack configuration

## 🧪 Testing

```bash
# Run tests
npm test

# Run tests with coverage
npm run test:coverage

# Run tests in watch mode
npm run test:watch
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Support

For support and questions:
- **Email**: support@synchrony-training.com
- **Slack**: #training-platform-support
- **Documentation**: Visit our internal wiki

## 📄 License

This project is proprietary software of Synchrony Financial. All rights reserved.

---

**Built with ❤️ for Synchrony Bank's global training initiative**

*Empowering agents worldwide through AI-driven empathy training*
