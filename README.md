# 🎓 Zest Academy

Welcome to **Zest Academy** - Your Gateway to Personalized Learning!

Zest Academy is a modern, interactive learning platform designed to provide students with comprehensive courses, curated roadmaps, and an intelligent chatbot assistant to guide their learning journey. Whether you're exploring new skills or mastering existing ones, Zest Academy offers a personalized experience tailored to your educational goals.

---

## ✨ Features

### 🏠 Home Page Sections

- **Courses Section** 📚
  - Browse through a comprehensive catalog of courses across various domains
  - Filter and search courses based on your interests and skill level
  - View course details, prerequisites, and learning outcomes

- **Explore Section** 🔍
  - Discover trending topics and emerging technologies
  - Personalized recommendations based on your profile and interests
  - Featured content curated by industry experts

- **Categories Section** 🗂️
  - Organized learning paths across multiple domains
  - Categories include: Web Development, Data Science, Mobile Development, AI/ML, Design, and more
  - Quick navigation to specific areas of interest

- **Roadmaps Section** 🗺️
  - Step-by-step learning paths for various career goals
  - Structured progression from beginner to advanced levels
  - Track your progress and achievements along the way

- **AI Chatbot Assistant** 🤖
  - 24/7 intelligent chatbot support
  - Get instant answers to your learning questions
  - Course recommendations and guidance
  - Help with navigation and platform features

### 🔐 Authentication & User Management

- **Multiple Sign-In Options**
  - Email/Password authentication
  - Google OAuth integration
  - Secure and seamless login experience

- **User Profile Information**
  - **Name**: Personal identification
  - **Current Class/Grade**: Educational level
  - **Skills to Learn**: Personalized learning goals and interests
  - Profile customization and preferences

### 🎨 Design System

#### Primary Color Scheme
- **Primary**: Gradient Blue
  - Linear gradient combining vibrant blue tones
  - Used for headers, CTAs, and primary interactive elements
  - Example: `linear-gradient(135deg, #667eea 0%, #764ba2 100%)`

#### Secondary Colors
- **Light Green** 🟢: Success states, positive feedback, completed items
- **Yellow** 🟡: Warnings, highlights, important information
- **Red** 🔴: Errors, alerts, critical notifications

#### Theme Support
- **Light Mode** ☀️
  - Background: White (#FFFFFF)
  - Clean, bright interface for daytime use
  
- **Dark Mode** 🌙
  - Background: Black (#000000) / Dark Grey (#1a1a1a)
  - Reduced eye strain for nighttime learning

---

## 🛠️ Technology Stack

### Recommended Frontend
- **Framework**: React.js / Next.js
- **Styling**: Tailwind CSS / Styled Components
- **State Management**: Redux / Context API
- **UI Components**: Material-UI / Ant Design / Chakra UI

### Recommended Backend
- **Server**: Node.js with Express.js / Python with FastAPI
- **Database**: MongoDB / PostgreSQL
- **Authentication**: Firebase Auth / Auth0 / Passport.js
- **API**: RESTful API / GraphQL

### Recommended Chatbot Integration
- **AI/ML**: OpenAI GPT API / Dialogflow / Rasa
- **Real-time Communication**: WebSocket / Socket.io

### Recommended Cloud Services
- **Hosting**: Vercel / Netlify / AWS / Google Cloud
- **Database**: MongoDB Atlas / AWS RDS / Supabase
- **Storage**: AWS S3 / Cloudinary (for media assets)

---

## 📁 Project Structure

```
zest-academy/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Home/
│   │   │   │   ├── CoursesSection.jsx
│   │   │   │   ├── ExploreSection.jsx
│   │   │   │   ├── CategoriesSection.jsx
│   │   │   │   ├── RoadmapsSection.jsx
│   │   │   │   └── Chatbot.jsx
│   │   │   ├── Auth/
│   │   │   │   ├── Login.jsx
│   │   │   │   ├── SignUp.jsx
│   │   │   │   └── GoogleAuth.jsx
│   │   │   ├── Profile/
│   │   │   │   └── UserProfile.jsx
│   │   │   ├── Layout/
│   │   │   │   ├── Header.jsx
│   │   │   │   ├── Footer.jsx
│   │   │   │   └── Navigation.jsx
│   │   │   └── shared/
│   │   │       ├── Button.jsx
│   │   │       ├── Card.jsx
│   │   │       └── ThemeToggle.jsx
│   │   ├── pages/
│   │   │   ├── Home.jsx
│   │   │   ├── Courses.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   └── Profile.jsx
│   │   ├── styles/
│   │   │   ├── theme.js
│   │   │   ├── colors.js
│   │   │   └── global.css
│   │   ├── utils/
│   │   ├── hooks/
│   │   ├── context/
│   │   └── App.jsx
│   ├── package.json
│   └── README.md
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   │   ├── User.js
│   │   │   ├── Course.js
│   │   │   └── Roadmap.js
│   │   ├── routes/
│   │   ├── middleware/
│   │   ├── config/
│   │   └── app.js
│   ├── package.json
│   └── README.md
├── chatbot/
│   ├── src/
│   │   ├── intents/
│   │   ├── training/
│   │   └── bot.js
│   └── README.md
├── docs/
│   ├── API.md
│   ├── DESIGN.md
│   └── DEPLOYMENT.md
├── .github/
│   └── workflows/
├── .gitignore
├── docker-compose.yml
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- MongoDB or PostgreSQL
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Zest-Academy/zest-academy.git
   cd zest-academy
   ```

2. **Install Frontend Dependencies**
   ```bash
   cd frontend
   npm install
   ```

3. **Install Backend Dependencies**
   ```bash
   cd backend
   npm install
   ```

4. **Environment Configuration**
   
   Create `.env` files in both frontend and backend directories:
   
   **Frontend `.env`:**
   ```env
   REACT_APP_API_URL=http://localhost:5000
   REACT_APP_GOOGLE_CLIENT_ID=your_google_client_id
   ```
   
   **Backend `.env`:**
   ```env
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   GOOGLE_CLIENT_ID=your_google_client_id
   GOOGLE_CLIENT_SECRET=your_google_client_secret
   OPENAI_API_KEY=your_openai_api_key
   ```

5. **Run the Application**
   
   **Development Mode:**
   ```bash
   # Terminal 1 - Backend
   cd backend
   npm run dev
   
   # Terminal 2 - Frontend
   cd frontend
   npm start
   ```
   
   **Production Mode:**
   ```bash
   # Build frontend
   cd frontend
   npm run build
   
   # Start backend with frontend
   cd backend
   npm start
   ```

6. **Access the Application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000
   - API Documentation: http://localhost:5000/api-docs

---

## 📖 Usage Guide

### For Students

1. **Create an Account**
   - Sign up using email or Google authentication
   - Complete your profile with name, current class, and skills you want to learn

2. **Explore Learning Content**
   - Browse the **Courses Section** for available courses
   - Use the **Explore Section** for personalized recommendations
   - Navigate through **Categories** to find specific topics
   - Follow **Roadmaps** for structured learning paths

3. **Use the Chatbot**
   - Click the chatbot icon in the bottom-right corner
   - Ask questions about courses, learning paths, or platform features
   - Get instant recommendations and support

4. **Track Your Progress**
   - View your dashboard for enrolled courses
   - Monitor your progress on roadmaps
   - Access your learning history and achievements

### For Administrators

1. **Content Management**
   - Add and update courses through the admin panel
   - Create and manage learning roadmaps
   - Organize content into categories

2. **User Management**
   - View user statistics and engagement
   - Monitor chatbot interactions
   - Generate reports on platform usage

---

## 🎨 Design Guidelines

### Color Usage

```css
/* Primary Gradient Blue */
.gradient-blue {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

/* Secondary Colors */
.success { color: #10b981; }  /* Light Green */
.warning { color: #fbbf24; }  /* Yellow */
.error { color: #ef4444; }    /* Red */

/* Theme Colors */
/* Light Mode */
.light-mode {
  --bg-primary: #ffffff;
  --text-primary: #1f2937;
  --text-secondary: #6b7280;
}

/* Dark Mode */
.dark-mode {
  --bg-primary: #000000;
  --text-primary: #f9fafb;
  --text-secondary: #d1d5db;
}
```

### Component Styling
- Use the gradient blue for primary buttons and headers
- Apply secondary colors for status indicators
- Ensure proper contrast ratios for accessibility
- Implement smooth theme transitions

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### How to Contribute

1. **Fork the Repository**
   ```bash
   git clone https://github.com/your-username/zest-academy.git
   ```

2. **Create a Feature Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes**
   - Follow the existing code style
   - Add tests for new features
   - Update documentation as needed

4. **Commit Your Changes**
   ```bash
   git commit -m "Add: Brief description of your changes"
   ```

5. **Push to Your Fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create a Pull Request**
   - Provide a clear description of your changes
   - Reference any related issues
   - Wait for review and feedback

### Code Style Guidelines

- Use ESLint and Prettier for code formatting
- Follow React best practices and hooks guidelines
- Write meaningful commit messages
- Add comments for complex logic
- Ensure responsive design for all components

### Testing

- Write unit tests for utility functions
- Add integration tests for API endpoints
- Test components with React Testing Library
- Ensure all tests pass before submitting PR

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📞 Contact & Support

- **Website**: https://zest-academy.com
- **Email**: support@zest-academy.com
- **Discord**: [Join our community](https://discord.gg/zest-academy)
- **Twitter**: [@ZestAcademy](https://twitter.com/ZestAcademy)

### Report Issues
If you encounter any bugs or have feature requests, please [open an issue](https://github.com/Zest-Academy/.github/issues) on GitHub.

---

## 🌟 Acknowledgments

- Thanks to all contributors who have helped build Zest Academy
- Special thanks to the open-source community for amazing tools and libraries
- Inspired by the vision of making quality education accessible to everyone

---

## 🗺️ Roadmap

### Upcoming Features
- [ ] Mobile application (iOS & Android)
- [ ] Live coding playground
- [ ] Peer-to-peer learning sessions
- [ ] Certificate generation upon course completion
- [ ] Integration with popular IDEs
- [ ] Video lectures and interactive tutorials
- [ ] Gamification and achievement badges
- [ ] Multi-language support

---

<div align="center">
  
  **Made with ❤️ by the Zest Academy Team**
  
  ⭐ Star us on GitHub if you find this project helpful!
  
</div>