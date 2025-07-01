# Admin UI Backend (In Development)

A Node.js/Express.js REST API backend service for an administrative user interface system <b>[admin-ui-angular](https://github.com/nlosinsky/admin-ui-angular)</b>. This backend provides authentication, user management, and business logic for managing companies, transactions, members, accounts, and documents.

## 🚀 Features

- **Authentication System** - JWT-based authentication with token verification
- **User Management** - Complete CRUD operations for user accounts
- **Company Management** - Handle company data and operations
- **Transaction Processing** - Manage financial transactions
- **Member Management** - Handle member registrations and profiles
- **Account Management** - Financial account operations
- **Document Management** - File and document handling
- **Constant Data** - Static data management (countries, etc.)

## 🛠️ Tech Stack

- **Runtime**: Node.js
- **Framework**: Express.js
- **Authentication**: JWT tokens
- **Data Storage**: JSON file-based database
- **CORS**: Cross-origin resource sharing
- **Development**: Nodemon for hot reloading

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/nlosinsky/admin-ui-backend.git
cd admin-ui-backend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The server will start on `http://localhost:3000`

## 🔧 API Endpoints

### Authentication
- `POST /auth` - User authentication

### Protected Routes (require JWT token)
- `GET/POST/PUT/DELETE /users` - User management
- `GET/POST/PUT/DELETE /companies` - Company management
- `GET/POST/PUT/DELETE /transactions` - Transaction management
- `GET/POST/PUT/DELETE /members` - Member management
- `GET/POST/PUT/DELETE /accounts` - Account management
- `GET/POST/PUT/DELETE /documents` - Document management

### Public Routes
- `GET /constant-data` - Static data (countries, etc.)

## 🔒 Security

- JWT token-based authentication
- CORS configured for specific origins
- Protected routes with middleware verification
- Cookie-based session management

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Note**: This is a backend service designed to work with a frontend admin UI. Make sure to configure the frontend to connect to the correct backend URL and handle authentication properly.
