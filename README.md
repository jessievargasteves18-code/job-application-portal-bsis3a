# 🚀 Job Posting Portal

A modern, full-featured job posting and management platform built with React, TypeScript, and Material UI. Connect employers with talented employees in a seamless, intuitive interface.

![Status](https://img.shields.io/badge/Status-Frontend%20UI%20Complete-green)
![Version](https://img.shields.io/badge/Version-0.1.0-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

## ✨ Features

### 🔐 Authentication System
- **Dual Role Support**: Separate workflows for Employees and Employers
- **Sign In Page**: Email/password login with role selection
- **Sign Up Page**: Multi-step registration process
- **Guest Login**: Quick access for browsing
- **Session Management**: Secure user sessions with Firebase

### 📊 Dashboards
- **Employee Dashboard**: Track saved jobs, applications, profile views, and offers
- **Employer Dashboard**: Manage job listings, applications, and hiring metrics
- **Role-Based Content**: Dynamic UI based on user role

### 🎨 User Interface
- **Material Design**: Professional, modern interface
- **Responsive Layout**: Perfect on mobile, tablet, and desktop
- **Intuitive Navigation**: Clear user flows and navigation
- **Smooth Animations**: Professional transitions and effects

---

## 🏗️ Project Structure

```
src/
├── config/
│   └── firebase.ts              # Firebase SDK configuration
├── pages/
│   ├── auth/
│   │   ├── SignIn.tsx          # Sign in page
│   │   └── SignUp.tsx          # Registration page
│   └── dashboard/
│       └── Dashboard.tsx        # Role-based dashboard
├── theme/
│   └── theme.ts                # Material UI theme
├── App.tsx                     # Main app component
├── main.tsx                    # React entry point
├── index.css                   # Global styles
└── vite-env.d.ts              # Type definitions
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| **React 18** | UI Framework |
| **TypeScript** | Type Safety |
| **Vite** | Build Tool |
| **Material UI** | Component Library |
| **React Router** | Navigation |
| **Firebase** | Authentication & Database |
| **Tailwind CSS** | Utility Styles |
| **Bun** | Package Manager |

---

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ or Bun installed
- Git

### Installation

1. **Clone the repository**
```bash
git clone <your-repo-url>
cd JobPostingPortal
```

2. **Install dependencies**
```bash
bun install
```

3. **Start development server**
```bash
bun run dev
```

4. **Open in browser**
Navigate to `http://localhost:5173`

---

## 📖 Documentation

This project includes comprehensive documentation:

| Document | Purpose |
|----------|---------|
| **QUICKSTART.md** | 30-second getting started guide |
| **FRONTEND_SETUP.md** | Technical setup details |
| **UI_PAGES_SUMMARY.md** | Visual descriptions of all pages |
| **SETUP_COMPLETE.md** | Complete setup documentation |
| **PROJECT_SUMMARY.md** | Project overview and status |
| **IMPLEMENTATION_CHECKLIST.md** | Development roadmap |

**Read first**: Start with `QUICKSTART.md` or `PROJECT_SUMMARY.md`

---

## 🎯 Features Overview

### Sign In Page (`/signin`)
- ✅ Role selection (Employee/Employer)
- ✅ Email and password login
- ✅ Guest login option
- ✅ Form validation
- ✅ Error handling
- ✅ Loading states

### Sign Up Page (`/signup`)
- ✅ Multi-step registration (3 steps)
- ✅ Role selection
- ✅ Personal information collection
- ✅ Account creation
- ✅ Form validation at each step
- ✅ Progress indicator

### Dashboards (`/dashboard/:role`)
- ✅ Employee dashboard with role-specific metrics
- ✅ Employer dashboard with hiring metrics
- ✅ Sign out functionality
- ✅ Responsive grid layout

---

## 📱 Responsive Design

Fully responsive across all devices:

- **Mobile** (< 600px): Single column layout
- **Tablet** (600-960px): Two column layout
- **Desktop** (960px+): Four column layout
- **Large Screens** (1280px+): Optimized container

---

## 🔐 Security Features

- ✅ Firebase authentication configured
- ✅ Environment variables for sensitive data
- ✅ Form validation
- ✅ Password field masking
- ✅ TypeScript for type safety
- ⏳ Protected routes (ready for implementation)
- ⏳ Session management (ready for implementation)

---

## 🎨 Design System

### Color Palette
```
Primary:      #667eea (Purple-Blue)
Secondary:    #764ba2 (Purple)
Success:      #10b981 (Green)
Warning:      #f59e0b (Amber)
Text Primary: #333333
Background:   #f5f5f5
```

### Typography
- **Font Family**: Segoe UI, Roboto, Oxygen, Ubuntu
- **Heading Weight**: 600-700
- **Body Weight**: 400-500
- **Line Height**: 1.5-1.6

---

## 📦 Commands

```bash
# Start development server with hot reload
bun run dev

# Build for production
bun run build

# Preview production build
bun run preview

# Run linting (setup required)
bun run lint
```

---

## 🔄 User Flows

### Sign In Flow
1. User lands on `/signin`
2. Selects role (Employee/Employer)
3. Enters email and password
4. Clicks "Sign In" or "Continue as Guest"
5. Navigates to `/dashboard/:role`

### Sign Up Flow
1. User clicks "Sign up" link
2. **Step 1**: Selects role
3. **Step 2**: Enters personal information
4. **Step 3**: Creates account
5. Navigates to `/dashboard/:role`

### Dashboard Flow
1. User views role-specific dashboard
2. Sees metrics and welcome message
3. Can sign out to return to login

---

## 🚧 Development Status

### ✅ Completed
- Frontend UI design and implementation
- Authentication pages
- Dashboard structure
- Material UI theme
- Responsive design
- Routing setup
- Form validation UI
- Documentation

### ⏳ In Progress
- Firebase authentication logic
- User session management
- Protected routes

### 📋 Upcoming
- User management system
- Job posting system
- Job applications
- Search and filtering
- Messaging system
- Email notifications
- Analytics dashboard

See `IMPLEMENTATION_CHECKLIST.md` for detailed development roadmap.

---

## 🎓 Learning & Resources

- [React Documentation](https://react.dev/)
- [Material UI Docs](https://mui.com/)
- [React Router Docs](https://reactrouter.com/)
- [Firebase Docs](https://firebase.google.com/docs/)
- [TypeScript Docs](https://www.typescriptlang.org/)
- [Vite Docs](https://vitejs.dev/)

---

## 📝 Environment Setup

Firebase credentials are configured in `.env`:

```env
VITE_FIREBASE_API_KEY=your_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
VITE_FIREBASE_MEASUREMENT_ID=your_measurement_id
```

See `.env.example` for template.

---

## 🤝 Contributing

This is a project under active development. The frontend UI is complete and ready for backend integration.

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 🎉 Get Started

1. Install dependencies: `bun install`
2. Start dev server: `bun run dev`
3. Read `QUICKSTART.md` for next steps
4. Explore the UI in your browser

---

## 📞 Support

- Check the documentation files (*.md) for detailed info
- Review the code comments for implementation details
- See `IMPLEMENTATION_CHECKLIST.md` for development guidance

---

## 🙌 Acknowledgments

- **Material UI**: For the component library
- **React Router**: For seamless navigation
- **Firebase**: For authentication infrastructure
- **Vite**: For the amazing build experience

---

**Happy Building! 🚀**

The foundation is solid. Let's build something amazing together!
