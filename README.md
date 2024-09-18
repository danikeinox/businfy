# Businfy

**Businfy** is a SaaS platform designed to automate the registration process of companies in Spain. It provides users with a simple and fast way to submit all necessary forms, upload documents, and verify identity. Once a company is registered, Businfy offers a freemium service for business management.

---

## Features

- **Company Registration Automation**: Simplifies legal company registration procedures (e.g., mercantile registry, food handling permits, trademarks).
- **Document Upload and Identity Verification**: Allows users to upload necessary documents and verifies identity through integrated services.
- **Freemium Business Management**: After company registration, users can manage:
  - Clients
  - Suppliers
  - Invoices
  - Estimates
  - Email campaigns with SEO analytics
  
  **Free Plan**: Limited usage of features like clients, invoices, and suppliers.

  **Paid Plans**: Include unlimited usage of features, with full access to marketing tools, client management, and automation.

---

## Tech Stack

- **Frontend**: React.js
- **Backend**: Node.js with Express.js
- **Database**: PostgreSQL
- **File Storage**: AWS S3 (or other cloud storage solutions)
- **Authentication**: JWT for user authentication and authorization
- **Containerization**: Docker for consistent development and deployment environments
- **API Management**: Token-based API access for developers

---

## Installation

### Prerequisites

- **Node.js** (v14 or higher)
- **PostgreSQL** (v12 or higher)
- **Docker** (optional, but recommended)

### Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/danikeinox/businfy.git
   cd businfy
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure environment variables**: Create a `.env` file with your configuration (e.g., database credentials, JWT secrets).
   ```bash
   DB_HOST=host
   DB_PORT=5432
   DB_USER=user
   DB_PASSWORD=password
   JWT_SECRET=jwt_secret
   ```

4. **Run the app**:
   ```bash
   npm start
   ```

### Docker Setup (Optional)

1. **Build Docker image**:
   ```bash
   docker build -t businfy .
   ```

2. **Run Docker container**:
   ```bash
   docker run -p 5000:5000 businfy
   ```

---

## API Endpoints

### User Authentication

- **POST /api/auth/register**: Register a new user
- **POST /api/auth/login**: Login an existing user

### Company Registration

- **POST /api/company/register**: Register a new company
- **GET /api/company/:id**: Get company details

### Business Management

- **POST /api/client/add**: Add a new client
- **GET /api/client/list**: List all clients
- **POST /api/invoice/create**: Create a new invoice
- **GET /api/invoice/list**: List all invoices

---

## Future Plans

- Integration with third-party email services for marketing
- SEO tools for campaign optimization
- Advanced analytics dashboard for premium users
- API marketplace for external developers

---

## License

This project is licensed under the **[MIT License](https://opensource.org/licenses/MIT)**.
