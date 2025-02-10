
# ProShop: Saka Motors E-Commerce Platform

**ProShop** is a comprehensive full-stack e-commerce platform built for **Saka Motors**, designed to streamline vehicle sales, services, and customer management. This project is developed using the **MERN stack** and includes robust backend functionality with extensive API coverage, making it a powerful tool for automotive businesses.

---

## Key Features

### Backend
- **Extensive API Coverage**: 
  - Product, user, admin, manager, store, mechanic, book, and auction management.
  - Specialized routes for uploads, bids, payments, and emails.
- **Session Management**: Secure session handling using `express-session`.
- **Error Handling**: Comprehensive middleware for `404` errors and global error handling.
- **Real-Time Data**: Enabled with `morgan` for detailed request logging in development.
- **Secure Payments**: Integrated PayPal and Stripe payment processing.
- **File Uploads**: Upload management for vehicle images, documents, and media using custom routes.

### Frontend
- **Dynamic User Experience**:
  - Modern UI components with `@coreui/react` and `@material-ui/core`.
  - Real-time updates and data visualization using carousels and charts (`react-elastic-carousel`, `recharts`).
- **Interactive Chatbot**: Integrated **Kommunicate Chatbot** for 24/7 customer assistance.

### Admin Features
- Manage products, orders, users, and services through a secure admin dashboard.
- Generate detailed sales and inventory reports, exportable using `jspdf` and `jspdf-autotable`.

### User Features
- Browse products, book services, and participate in auctions.
- Real-time bid management and notifications using `socket.io`.

### Additional Functionalities
- **Flash Messaging**: Using `connect-flash` for enhanced user feedback.
- **CORS Support**: Cross-origin requests enabled for flexible frontend-backend communication.
- **Multiple Routes**: Modularized structure to support scaling and feature expansion.

---

## Tech Stack

- **Frontend**: React, Material-UI, CoreUI
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JSON Web Tokens (JWT)
- **Payment Gateway**: Stripe, PayPal
- **File Uploads**: Multer, Sharp
- **Real-Time Communication**: Socket.IO
- **Chatbot**: Kommunicate

---

## Installation and Setup

### Prerequisites
- Node.js (v16.17.x)
- MongoDB (local or cloud instance)
- PayPal and Stripe developer accounts

### Steps to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/proshop.git
   cd proshop
   ```

2. Install dependencies:
   ```bash
   npm install
   npm install --prefix frontend
   ```

3. Configure environment variables:
   Create a `.env` file in the root directory and specify:
   - `MONGO_URI`: MongoDB connection string
   - `JWT_SECRET`: Secret key for authentication
   - `PAYPAL_CLIENT_ID`: PayPal API client ID
   - `STRIPE_SECRET_KEY`: Stripe API secret key

4. Start the development server:
   ```bash
   npm run dev
   ```

   This will start both the frontend and backend servers concurrently.

---

## Deployment

The project is preconfigured for deployment on platforms like **Heroku**. The `heroku-postbuild` script ensures the frontend is built and ready for production.

---

## API Overview

### Public Routes
- **Products**: `GET /api/products/`
- **Auctions**: `GET /api/auctions/`
- **Posts**: `GET /api/posts/`

### Admin Routes
- **Users Management**: `GET /api/admins/`
- **Product Management**: `POST /api/aproducts/`
- **Store Management**: `GET /api/astores/`

### Payment Routes
- **Stripe**: `POST /api/pay/stripe`
- **PayPal Configuration**: `GET /api/config/paypal`

### File Uploads
- **User Uploads**: `POST /api/upload/`
- **Manager Uploads**: `POST /api/uploadm/`

### Communication Routes
- **Emails**: `POST /api/email/send`


---

## Future Enhancements
- **AI-Powered Recommendations**: Implement AI for personalized vehicle suggestions.
- **Advanced Analytics**: Add more business insights and forecasting tools.
- **Push Notifications**: Notify users of auctions, bids, and offers in real time.

---
## Screenshots

![Screenshot 1](screenshots/sccrn 1.jpeg)
![Screenshot 1](screenshots/sccrn 2.jpeg)
![Screenshot 1](screenshots/sccrn 3.jpeg)
![Screenshot 1](screenshots/sccrn 4.jpeg)



## Credits

Developed by **Joseph James K.**, showcasing expertise in backend development, API design, and full-stack integration.

---
