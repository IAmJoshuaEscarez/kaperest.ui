# ☕ KapeRest UI

[![React](https://img.shields.io/badge/React-18.0+-blue)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.0+-purple)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.0+-38B2AC)](https://tailwindcss.com/)

React frontend for the KapeRest café management system, built with TypeScript, Vite, and Tailwind CSS.

## � Related Repositories

| Repository | Description | Technology | Link |
|------------|-------------|------------|------|
| **KapeRest Backend** | ASP.NET Core Web API with Clean Architecture | C# .NET 9.0 | [GitHub](https://github.com/Jesc06/KapeRest.Api.git) |

> **Note**: This frontend requires the backend API to be running. See the backend repository for API setup instructions.

## �📋 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Prerequisites](#-prerequisites)
- [Installation](#-installation)
- [Configuration](#-configuration)
- [Usage](#-usage)
- [Development](#-development)
- [Building for Production](#-building-for-production)
- [Contributing](#-contributing)
- [License](#-license)

## ⚙️ Features

- **Modern UI/UX**: Clean, responsive design with Tailwind CSS
- **TypeScript**: Full type safety and better developer experience
- **Fast Development**: Vite for lightning-fast hot module replacement
- **POS Interface**: Intuitive point-of-sale system for café operations
- **Inventory Management**: Real-time stock tracking and alerts
- **User Management**: Role-based access control
- **Analytics Dashboard**: Sales reports and business insights
- **Payment Integration**: GCash payment processing
- **Real-time Updates**: Live notifications and data synchronization

## 🧩 Tech Stack

| Component       | Technology                              |
|-----------------|-----------------------------------------|
| **Framework**   | React 18+                               |
| **Language**    | TypeScript                              |
| **Build Tool**  | Vite                                    |
| **Styling**     | Tailwind CSS                            |
| **State Mgmt**  | React Context API                       |
| **HTTP Client** | Axios                                   |
| **Routing**     | React Router                            |
| **Icons**       | Lucide React                            |
| **Backend API** | KapeRest ASP.NET Core API               |

## 📋 Prerequisites

- [Node.js 18+](https://nodejs.org/) (LTS version recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [Git](https://git-scm.com/)
- Running KapeRest backend API (see main README)

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/KapeRest.git
   cd KapeRest.UI
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```
   or
   ```bash
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```
   or
   ```bash
   yarn dev
   ```

The application will be available at `http://localhost:5173`.

## ⚙️ Configuration

### Environment Variables

Create a `.env` file in the root directory:

```env
# Backend API Configuration
VITE_API_BASE_URL=https://localhost:5001/api

# App Configuration
VITE_APP_NAME=KapeRest
VITE_APP_VERSION=1.0.0
```

### Backend Connection

Ensure the KapeRest backend API is running and accessible. The frontend expects the API to be available at the URL specified in `VITE_API_BASE_URL`.

## 📖 Usage

1. **Start the backend API** (from the main KapeRest directory):
   ```bash
   cd ../KapeRest.Api
   dotnet run
   ```

2. **Start the frontend** (from KapeRest.UI directory):
   ```bash
   npm run dev
   ```

3. **Access the application**:
   - Open `http://localhost:5173` in your browser
   - Log in with admin credentials (see backend README)

### Default Login Credentials
- **Email**: admin@kaperest.com
- **Password**: Admin@123456

## 🛠️ Development

### Available Scripts

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run linting
npm run lint

# Format code
npm run format
```

### Project Structure

```
src/
├── components/          # Reusable UI components
├── pages/              # Page components
├── services/           # API service functions
├── context/            # React context providers
├── utils/              # Utility functions
├── hooks/              # Custom React hooks
├── types/              # TypeScript type definitions
├── config/             # Configuration files
└── assets/             # Static assets
```

### Code Style

This project uses ESLint and Prettier for code formatting. Run `npm run lint` to check for issues and `npm run format` to auto-format code.

## 🏗️ Building for Production

1. **Build the application**:
   ```bash
   npm run build
   ```

2. **Preview the build**:
   ```bash
   npm run preview
   ```

3. **Deploy the `dist` folder** to your web server or hosting platform.

## 🔧 Troubleshooting

### Common Issues

- **Backend connection failed**: Ensure the KapeRest API is running and the URL in `.env` is correct
- **Port 5173 in use**: Change the port in `vite.config.ts` or use `npm run dev -- --port 3000`
- **Build errors**: Run `npm install` to ensure all dependencies are installed
- **CORS errors**: Check backend CORS configuration in `Program.cs`

### Development Tips

- Use browser developer tools to inspect network requests
- Check the browser console for error messages
- Ensure TypeScript types are properly defined
- Test API endpoints using Swagger UI first

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines

- Follow the existing code style and structure
- Write meaningful commit messages
- Add TypeScript types for new features
- Test your changes thoroughly
- Update documentation as needed

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](../LICENSE) file for details.

---

Built with ❤️ for the KapeRest café management system.
