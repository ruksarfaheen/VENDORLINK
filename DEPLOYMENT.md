# VendorLink Deployment Guide

## 🚀 Quick Deployment

### Prerequisites
- Node.js 20 or higher
- npm or yarn package manager

### Download & Setup

#### Option 1: Download as ZIP
1. Click the "Download" button in Replit or use the export feature
2. Extract the ZIP file to your desired location
3. Open terminal in the project directory

#### Option 2: Clone Repository
```bash
git clone <your-repository-url>
cd vendorlink
```

### Installation Steps

1. **Install Dependencies**
   ```bash
   npm install
   ```

2. **Start Development Server**
   ```bash
   npm run dev
   ```

3. **Access Application**
   - Open your browser to `http://localhost:5000`
   - The application will be running with full functionality

### Production Deployment

#### Deploy to Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts to deploy

#### Deploy to Netlify
1. Build the project: `npm run build`
2. Upload the `dist` folder to Netlify
3. Configure redirects for SPA routing

#### Deploy to Railway/Render
1. Connect your Git repository
2. Set build command: `npm run build`
3. Set start command: `npm start`

### Environment Variables
No additional environment variables needed for basic functionality.

### Features Included
- ✅ Full-stack React + Express application
- ✅ In-memory database (no setup required)
- ✅ Real-time WebSocket chat
- ✅ Responsive design
- ✅ Sample data pre-loaded
- ✅ Zomato-inspired UI with yellow-black theme

### File Structure
```
vendorlink/
├── client/          # React frontend
├── server/          # Express backend
├── shared/          # Shared schemas and types
├── package.json     # Dependencies and scripts
└── vite.config.ts   # Build configuration
```

### Troubleshooting
- If port 5000 is busy, the app will automatically use the next available port
- Ensure Node.js version is 20 or higher
- All data is stored in memory - it resets when the server restarts

### Support
Contact support for any deployment issues or customization needs.