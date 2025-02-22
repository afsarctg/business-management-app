# Setup Guide

## Prerequisites
1. Node.js (version 14 or higher)
2. npm or yarn package manager
3. Git
4. Visual Studio Code (recommended)
5. Firebase account

## Step 1: Initial Setup

### Install Development Tools
```bash
# Check Node.js installation
node --version
npm --version

# Install Firebase tools
npm install -g firebase-tools

# Install React development tools
npm install -g create-react-app
```

### Clone the Repository
```bash
git clone https://github.com/your-username/business-management-app.git
cd business-management-app
```

## Step 2: Environment Configuration

### Create Environment Files
```bash
# Create development environment file
cp .env.example .env.development

# Create production environment file
cp .env.example .env.production
```

### Configure Firebase
1. Go to Firebase Console
2. Create new project
3. Get configuration details
4. Update `.env` files with Firebase details

## Step 3: Installation

### Install Dependencies
```bash
# Install project dependencies
npm install

# Additional dependencies
npm install @firebase/app @firebase/auth @firebase/firestore
npm install react-router-dom tailwindcss @headlessui/react
npm install recharts i18next react-i18next
```

## Step 4: Database Setup

### Firebase Configuration
1. Enable Authentication
   - Go to Firebase Console
   - Set up Email/Password authentication
   - Configure OAuth providers if needed

2. Create Firestore Database
   - Set up Firestore in Firebase Console
   - Configure security rules
   - Set up initial collections

## Step 5: Development Server

### Run the Application
```bash
# Start development server
npm start

# Run tests
npm test

# Create production build
npm run build
```

## Troubleshooting

### Common Issues
1. Node version mismatch
   - Solution: Use nvm to manage Node versions

2. Dependencies issues
   - Solution: Delete node_modules and package-lock.json
   - Run: npm install

3. Environment variables not loading
   - Check .env file location
   - Verify variable names start with REACT_APP_

## Next Steps
1. Review deployment guide
2. Set up CI/CD pipeline
3. Configure monitoring tools
4. Set up backup procedures