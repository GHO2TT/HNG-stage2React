# TicketApp 🎫

A modern, responsive ticket management system built with React and Vite. This application provides a complete solution for managing support tickets with user authentication, CRUD operations, and real-time status tracking.

## ✨ Features

- **User Authentication**: Secure login and signup system with session management
- **Protected Routes**: Role-based access control for authenticated users
- **Ticket Management**: Create, read, update, and delete tickets
- **Status Tracking**: Filter tickets by status (Open, In Progress, Closed)
- **Priority Levels**: Organize tickets with priority indicators (Low, Medium, High)
- **Toast Notifications**: Real-time feedback for user actions
- **Responsive Design**: Mobile-first, accessible UI with dark theme support
- **Modern UI Components**: Powered by shadcn/ui and Tailwind CSS

## 🚀 Tech Stack

- **Frontend Framework**: React 18
- **Build Tool**: Vite
- **Routing**: React Router v6
- **Styling**: Tailwind CSS with dark theme
- **UI Components**: shadcn/ui, Lucide Icons
- **Notifications**: React Toastify
- **State Management**: Local storage simulation
- **Language**: JavaScript/TypeScript

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- Node.js 16+
- npm, yarn, or pnpm package manager

## 🛠️ Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd ticket-appReactt
```

2. Install dependencies:

```bash
npm install
```

## 🏃 Running the Project

### Development Mode

Start the development server with hot reload:

```bash
npm run dev
```

The application will be available at `http://localhost:5173`

### Production Build

Build the application for production:

```bash
npm run build
```

### Preview Production Build

Preview the production build locally:

```bash
npm run preview
```

## 📁 Project Structure

```
ticket-appReactt/
├── app/                      # Next.js-style app router (legacy/hybrid)
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components/               # Reusable UI components
│   ├── ui/                   # shadcn-style components
│   └── theme-provider.tsx
├── src/                      # Main application source
│   ├── components/           # React components
│   │   ├── Footer.jsx
│   │   ├── Navbar.jsx
│   │   ├── ProtectedRoute.jsx
│   │   ├── TicketForm.jsx
│   │   └── TicketList.jsx
│   ├── pages/                # Page-level components
│   │   ├── Dashboard.jsx
│   │   ├── Landing.jsx
│   │   ├── Login.jsx
│   │   ├── Signup.jsx
│   │   └── Tickets.jsx
│   ├── services/             # Business logic
│   │   ├── authService.js    # Authentication service
│   │   └── ticketService.js  # Ticket management service
│   ├── App.jsx               # Main app component
│   ├── main.jsx              # Entry point
│   └── index.css             # Global styles
├── hooks/                    # Custom React hooks
├── lib/                      # Utility functions
└── styles/                   # Additional stylesheets
```

## 🔐 Authentication

The application uses **localStorage** for session management:

- **Session Key**: `ticketapp_session`
- **Users Key**: `ticketapp_users`

> **Note**: This is a simulated authentication system for demonstration purposes. For production use, implement proper backend authentication with secure token management.

## 🗺️ Routes

| Route          | Access    | Description       |
| -------------- | --------- | ----------------- |
| `/`            | Public    | Landing page      |
| `/auth/login`  | Public    | User login        |
| `/auth/signup` | Public    | User registration |
| `/dashboard`   | Protected | User dashboard    |
| `/tickets`     | Protected | Ticket management |

## 🎨 UI Components

The project includes a comprehensive set of UI components from shadcn/ui:

- Buttons, Inputs, Forms
- Dialogs, Alerts, Toasts
- Tables, Cards, Badges
- Navigation, Menus, Sidebars
- Charts, Calendars, Carousels
- And many more...

## 🧪 Key Features Explained

### Ticket Management

- Create new tickets with title, description, priority, and status
- Update existing tickets
- Delete unwanted tickets
- Filter tickets by status
- Priority-based color coding

### User Experience

- Responsive design that works on all devices
- Dark theme support
- Accessible components following WCAG guidelines
- Smooth transitions and animations
- Real-time toast notifications

## 🔧 Configuration Files

- `vite.config.js` - Vite configuration
- `tailwind.config.js` - Tailwind CSS configuration
- `tsconfig.json` - TypeScript configuration
- `postcss.config.js` - PostCSS configuration
- `components.json` - shadcn/ui component configuration

## 📦 Build Output

Production builds are output to the `dist/` directory and can be deployed to any static hosting service.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License.

## 🐛 Known Issues

- Authentication is simulated using localStorage (not suitable for production)
- No backend integration (data persists only in browser)

## 🔮 Future Enhancements

- Backend API integration
- Real authentication with JWT tokens
- Database persistence
- Email notifications
- File attachments for tickets
- Advanced filtering and search
- Analytics dashboard
- User roles and permissions

## 📧 Support

For support, please open an issue in the repository.

---

Built with ❤️ using React and Vite
