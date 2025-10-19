TaskMaster - React Task Management Application

A modern, responsive task management application built with React, Vite, and Tailwind CSS. Features dark mode, local storage persistence, and API integration.

Live link: https://task-master-three-inky.vercel.app/

https://img.shields.io/badge/React-18.2.0-blue
https://img.shields.io/badge/Vite-5.0.0-purple
https://img.shields.io/badge/Tailwind-3.3.0-cyan
 Features
 Core Functionality

    Task Management: Create, complete, delete, and filter tasks

    Local Storage: Tasks persist between browser sessions

    Dark/Light Mode: Toggle between themes with system preference detection

    Responsive Design: Works seamlessly on desktop, tablet, and mobile

 Advanced Features

    API Integration: Fetch and display user data from JSONPlaceholder API

    Real-time Search: Filter users by name, email, or company

    Infinite Scroll: Load more users as you scroll

    Custom Hooks: Reusable hooks for local storage and API calls

    Component Architecture: Modular, reusable UI components

 UI/UX

    Modern Design: Clean, intuitive interface with smooth animations

    Accessibility: Focus management and ARIA labels

    Loading States: Elegant loading indicators and error handling

    Interactive Elements: Hover effects and transitions

 Tech Stack

    Frontend: React 18, JSX

    Build Tool: Vite

    Styling: Tailwind CSS

    Routing: React Router DOM

    State Management: React Hooks (useState, useEffect, useContext)

    API: JSONPlaceholder REST API

    Icons: Unicode emojis and symbols

 Installation
Prerequisites

Make sure you have the following installed on your system:

    Node.js (version 14 or higher)

    npm or yarn package manager

Step-by-Step Setup

    Clone the repository
    bash

git clone <your-repository-url>
cd react-task-manager

Install dependencies
bash

npm install

or if using yarn:
bash

yarn install

Start the development server
bash

npm run dev

or with yarn:
bash

yarn dev

    Open your browser
    Navigate to http://localhost:5173 to view the application

 Project Structure
text

src/
├── components/          # Reusable UI components
│   ├── Button.jsx      # Button with variants (primary, secondary, danger)
│   ├── Card.jsx        # Card container for content
│   ├── Navbar.jsx      # Navigation header with theme toggle
│   ├── Footer.jsx      # Site footer with links
│   ├── Layout.jsx      # Main layout wrapper
│   ├── TaskManager.jsx # Task management functionality
│   └── UserList.jsx    # User list with search and pagination
├── context/            # React context providers
│   └── ThemeContext.jsx # Dark/light theme management
├── hooks/              # Custom React hooks
│   ├── useLocalStorage.js # Persist state to localStorage
│   └── useApi.js       # API data fetching with pagination
├── pages/              # Page components
│   └── Home.jsx        # Landing page
├── App.jsx             # Main app component with routing
├── main.jsx            # React DOM entry point
└── index.css           # Global styles and Tailwind imports

 Usage Guide
Task Management

    Add Tasks: Use the input field in the Task Manager page

    Complete Tasks: Click the checkbox next to any task

    Delete Tasks: Click the "Delete" button on any task

    Filter Tasks: Use the filter buttons (All, Active, Completed)

    Clear Completed: Remove all completed tasks at once

User Directory

    Browse Users: View all users from the JSONPlaceholder API

    Search Users: Use the search bar to filter by name, email, or company

    Load More: Click "Load More Users" to paginate through results

Theme Customization

    Click the theme toggle button in the navbar to switch between light and dark mode

    Your preference is saved automatically

 Customization
Adding New Components

    Create your component in the src/components/ directory

    Export it as a default export

    Import and use it in your pages

Styling with Tailwind

The project uses Tailwind CSS for styling. You can:

    Use utility classes directly in components

    Extend the theme in tailwind.config.js

    Add custom CSS in src/index.css

Adding New Pages

    Create a new component in src/pages/

    Add the route in src/App.jsx

    Update the navigation in src/components/Navbar.jsx

 Responsive Breakpoints

    Mobile: < 768px

    Tablet: 768px - 1024px

    Desktop: > 1024px

 Color Scheme
Light Mode

    Primary: Blue-600

    Background: Gray-50

    Text: Gray-900

    Cards: White

Dark Mode

    Primary: Blue-500

    Background: Gray-900

    Text: White

    Cards: Gray-800

 API Integration

The application integrates with the JSONPlaceholder API to demonstrate:

    Data fetching with useEffect

    Loading and error states

    Search functionality

    Pagination/infinite scroll

API Endpoints Used

    GET /users - Fetch user data

    Query parameters: _page, _limit for pagination

 Available Scripts
bash

# Development
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build

# Code Quality
npm run lint         # Run ESLint

 Deployment
Build for Production
bash

npm run build

The dist folder will contain the optimized production build ready for deployment.
Deployment Options

    Vercel: Connect your GitHub repository for automatic deployments

    Netlify: Drag and drop the dist folder

    GitHub Pages: Use the gh-pages package

    Traditional Hosting: Upload the dist folder to any web server

 Contributing

    Fork the repository

    Create a feature branch: git checkout -b feature/amazing-feature

    Commit your changes: git commit -m 'Add amazing feature'

    Push to the branch: git push origin feature/amazing-feature

    Open a pull request

 Code Guidelines

    Use functional components with hooks

    Follow React best practices

    Use meaningful component and variable names

    Keep components small and focused

    Use Tailwind CSS for styling

    Implement proper error handling

 Troubleshooting
Common Issues

    Port already in use
    bash

# Kill process on port 5173
npx kill-port 5173
# Or use different port
npm run dev -- --port 3000

Dependencies not installing
bash

# Clear cache and reinstall
npm cache clean --force
rm -rf node_modules package-lock.json
npm install

    Build errors

        Check Node.js version (requires 14+)

        Ensure all files are properly imported

        Verify component exports

 License

This project is open source and available under the MIT License.
 Acknowledgments

    React - UI library

    Vite - Build tool

    Tailwind CSS - CSS framework

    JSONPlaceholder - Fake API for testing

 Support

If you encounter any issues or have questions:

    Check the troubleshooting section above

    Search existing GitHub issues

    Create a new issue with detailed information

Happy coding!
