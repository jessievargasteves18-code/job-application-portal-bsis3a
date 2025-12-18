# UI Pages Summary - Job Posting Portal

## 🔐 Authentication Pages

### 1. Sign In Page (`/signin`)
**Visual Elements:**
- black/violet gradient background
- White card with shadow
- Brand header (JobPortal)
- Role toggle buttons (Employee / Employer)
  - Employee icon + label
  - Employer icon + label
- Form fields:
  - Email input
  - Password input
- Buttons:
  - "Sign In" (primary button, gradient background)
  - "Continue as Guest" (secondary button)
- Navigation:
  - Link to Sign Up page
- Footer: Copyright text

**User Flow:**
1. User enters on sign in page
2. Selects role (Employee or Employer)
3. Enters email and password
4. Clicks Sign In or Continue as Guest
5. Navigates to role-specific dashboard

---

### 2. Sign Up Page (`/signup`)
**Visual Elements:**
- Same gradient background as Sign In
- White card with shadow
- Brand header (JobPortal)
- Multi-step stepper
  - Step 1: Select Role
  - Step 2: Personal Info
  - Step 3: Account Details

**Step 1: Role Selection**
- Larger toggle buttons with icons and descriptions
- Employee: "Looking for jobs"
- Employer: "Hiring talent"

**Step 2: Personal Information**
- First Name input field
- Last Name input field
- Company Name input field (only for Employers)
- Back/Next buttons

**Step 3: Account Details**
- Email input field
- Password input field (with helper text: "At least 8 characters")
- Confirm Password input field
- Terms & Conditions checkbox
- Back/Create Account buttons

**Navigation:**
- Back button (disabled on first step)
- Next button (steps 1-2)
- Create Account button (step 3)
- Link to Sign In page
- Progress indicator (Stepper)

**User Flow:**
1. User lands on Sign Up
2. Selects role (Step 1)
3. Enters personal information (Step 2)
4. Enters account credentials (Step 3)
5. Creates account and navigates to dashboard

---

## 📊 Dashboard Pages

### 3. Employee Dashboard (`/dashboard/employee`)
**Visual Elements:**
- Header with:
  - Brand name (JobPortal)
  - Dashboard title "Employee Dashboard"
  - Sign Out button
- Welcome card with greeting message
- 4 metric cards in responsive grid:
  - Saved Jobs (purple)
  - Applications (secondary purple)
  - Profile Views (amber/orange)
  - Offers (green)
- Coming Soon card for future features

**Layout:**
- Container max-width: 1200px
- Responsive grid: 1 col (mobile) → 2 cols (tablet) → 4 cols (desktop)
- Each card shows metric name and count (0 as placeholder)

---

### 4. Employer Dashboard (`/dashboard/employer`)
**Visual Elements:**
- Same header structure as Employee Dashboard
- Different welcome message for employers
- 4 different metric cards:
  - Active Listings (purple)
  - Total Applications (secondary purple)
  - Pending Review (amber/orange)
  - Hired (green)
- Same Coming Soon card

**Layout:**
- Identical responsive grid structure
- Role-specific metrics and descriptions

---

## 🎨 Design System

### Colors
- **Primary**: #667eea (Purple-Blue)
- **Secondary**: #764ba2 (Purple)
- **Success**: #10b981 (Green)
- **Warning**: #f59e0b (Amber)
- **Text Primary**: #333333
- **Text Secondary**: #666666
- **Background**: #f5f5f5
- **Paper/Card**: #ffffff

### Typography
- **Font Family**: Segoe UI, Roboto, Oxygen, Ubuntu, sans-serif
- **Headings**: Bold weights (600-700)
- **Body**: Regular (400) and medium (500) weights
- **Line Heights**: 1.6 for body, 1.5 for smaller text

### Spacing
- Standard padding: 16px, 24px, 32px
- Gap between cards: 24px
- Container max-width: 1200px

### Components Used
- **Material UI Cards**: For containing content
- **Material UI TextFields**: For form inputs
- **Material UI Buttons**: For actions
- **Material UI ToggleButtons**: For role selection
- **Material UI Stepper**: For multi-step form
- **Material UI Typography**: For all text
- **Material UI Icons**: For visual elements (Person, Business, Logout)
- **Material UI Box**: For layout containers

### Responsive Breakpoints
- **Mobile**: xs (< 600px)
- **Tablet**: sm (600-960px)
- **Laptop**: md (960px+)
- **Desktop**: lg (1280px+)

---

## 🔄 Navigation Map

```
Sign In Page (/signin)
    ├─ [Sign In] → Employee Dashboard (/dashboard/employee)
    ├─ [Sign In] → Employer Dashboard (/dashboard/employer)
    ├─ [Continue as Guest] → Role-based Dashboard
    └─ [Sign Up Link] → Sign Up Page (/signup)

Sign Up Page (/signup)
    ├─ Step 1: Role Selection
    ├─ Step 2: Personal Info
    ├─ Step 3: Account Details
    └─ [Create Account] → Role-based Dashboard

Dashboard (/dashboard/:role)
    ├─ Employee Dashboard
    │   └─ [Sign Out] → Sign In Page
    └─ Employer Dashboard
        └─ [Sign Out] → Sign In Page

Root (/)
    └─ Redirect to Sign In Page
```

---

## 🚀 Ready for Implementation

All UI pages are built and ready for:
1. Firebase authentication logic
2. Form validation and submission
3. User session management
4. API integration for dashboard metrics
5. Protected routes and auth guards
