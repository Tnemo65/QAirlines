# QAirlines

## Overview

QAirline needs to develop a website to provide information about flights and services offered by the airline. At the same time, customers can book flights on QAirline's website.

## Features

- User registration and login (with JWT authentication).
- Flight search and booking.
- View and manage user bookings.
- Notifications for flight delays.
- Admin functionalities for managing flights and users.

## Technology Stack

- **Frontend**: React.js with [shadcn/ui](https://github.com/shadcn-ui/ui) components.
- **Backend**: Node.js with Express.js.
- **Database**: MongoDB.
- **Styling**: Tailwind CSS.

## Folder Structure

```
QAirlines/
├── client/          # Frontend code
├── server/          # Backend code
│   ├── controllers/ # API controllers
│   ├── models/      # Mongoose models
│   ├── routes/      # API routes
│   └── utils/       # Utility functions
└── README.md        # Project documentation
```

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/duongduc025/QAirlines.git
   cd QAirlines
   ```

2. Install and run the backend:
   ```
   cd server
   npm install
   npm start
   ```

3. Install and run the frontend:
   ```
   cd client
   npm install
   npm run dev
   ```

4. Access the application at `http://localhost:3000`.

## API Endpoints

### Authentication
- `POST /api/register`: Register a new user.
- `POST /api/login`: Login with email and password.
- `POST /api/loginWithToken`: Login using a JWT token.

### User Management
- `PUT /api/users/:id`: Update user information.
- `PUT /api/users/:id/changePassword`: Change user password.

### Bookings
- `GET /api/bookings`: List all bookings for a user.
- `POST /api/bookings`: Create a new booking.

### Notifications
- `GET /api/users/:id/delayNotices`: Get delay notices for a user.
- `PUT /api/users/:id/delayNotices`: Mark delay notices as viewed.

## Contribution Guidelines

1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```
   git commit -m "Add feature-name"
   ```
4. Push to your branch:
   ```
   git push origin feature-name
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
