# Super Admin Panel

A fully responsive, modern, and attractive Super Admin Panel built with React, TailwindCSS v4, Framer Motion, and Lucide Icons.

## Features

### Authentication (UI only)
- Login, Signup, Forgot Password pages
- Animated transitions between forms

### Dashboard
- KPI cards with animated counters (Users, Jobs, Applications, Institutions, Mentors)
- Interactive charts (line, bar, donut) using mock data
- Quick action buttons (e.g., Add User, Create Job) → open modals with working forms

### Sidebar + Navbar
- Collapsible sidebar with icons + tooltips
- Responsive: sidebar collapses to icons on mobile
- Top navbar with search bar, notification bell (opens drawer), user profile dropdown
- Dark mode toggle (saved in local storage)

### Users Management
- Data table with mock user data
- Search, sort, filter, pagination (all working on mock data)
- Row actions: Edit, Delete (open modal/drawer, update local state)
- Bulk actions (select multiple users, delete/activate)

### Institutions / Placement Cells
- Card + table view with dummy data
- Buttons: Verify, Assign Mentor (open modal, update mock state)
- Filters: by status (verified, pending)

### Mentors
- List of mentors with approval/rejection buttons
- Buttons trigger status updates with animations
- Drawer to show mentor profile

### Jobs & Placements
- Job postings list with status badges (active, closed)
- CRUD buttons: Add, Edit, Delete (modals with forms + state updates)
- Applications per job → expandable table view

### Applications
- Student applications with status pipeline (Applied → Shortlisted → Offered → Placed)
- Drag-and-drop style pipeline board (Kanban style with mock state)

### Audit Logs
- Timeline or table view with mock logs
- Filters: by date, user, action
- Export button (downloads JSON/CSV mock file)

### Settings
- Role & permission editor (checkboxes/toggles)
- Theme customization (colors, logo upload — mock only)
- Working save button (updates mock state)

### Notifications
- Bell icon opens a right drawer
- List of notifications (mark as read, clear all)
- Buttons update mock state in real time

### Profile Page
- Editable profile form with mock user info
- Avatar upload (preview only, no backend)
- Save button updates local state

## UI/UX Design Guidelines

- Use modern glassmorphism/neumorphism style (soft shadows, rounded corners, gradients)
- Smooth animations: sidebar toggle, modal open/close, hover effects, button clicks
- Use icons instead of long labels where possible (with tooltips)
- Responsive grid layout for cards and tables
- Light & Dark mode with elegant transitions
- Loading states & skeletons for tables and cards

## Tech Stack

- **Frontend**: React + Vite
- **Styling**: TailwindCSS v4
- **Animations**: Framer Motion
- **Icons**: Lucide Icons
- **Routing**: React Router DOM

## Folder Structure

```
src/
├── components/        # Reusable UI components
├── views/             # Page components
│   ├── auth/          # Authentication pages
│   ├── dashboard/     # Dashboard components
│   ├── users/         # Users management
│   ├── institutions/  # Institutions management
│   ├── mentors/       # Mentors management
│   ├── jobs/          # Jobs management
│   ├── applications/  # Applications management
│   ├── audit/         # Audit logs
│   ├── settings/      # Settings pages
│   └── profile/       # Profile page
├── layouts/           # Layout components
├── hooks/             # Custom hooks
├── utils/             # Utility functions
└── data/              # Mock data
```

## Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Available Scripts

- `npm run dev` - Starts the development server
- `npm run build` - Builds the production-ready app
- `npm run preview` - Previews the production build locally

## Dependencies

- react
- react-dom
- react-router-dom
- tailwindcss
- framer-motion
- lucide-react

## Development

This project uses Vite for fast development and Hot Module Replacement (HMR). All components are built with modern React patterns and hooks for state management.

## License

This project is licensed under the MIT License.