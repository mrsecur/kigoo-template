# Installation Instructions for Kigoo Template

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (vX.X.X)
- npm (vX.X.X) or yarn
- MySQL/PostgreSQL (depending on your database choice)
- Docker (if using containers)

## Frontend Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mrsecur/kigoo-template.git
   cd kigoo-template/frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install   # or yarn install
   ```

3. **Run the development server:**
   ```bash
   npm start     # or yarn start
   ```

4. **Open your browser and navigate to:**
   ```
   http://localhost:3000
   ```

## Backend Setup

1. **Navigate to the backend directory:**
   ```bash
   cd ../backend
   ```

2. **Install dependencies:**
   ```bash
   npm install   # or yarn install
   ```

3. **Create a `.env` file based on the `.env.example`:**
   ```bash
   cp .env.example .env
   ```

4. **Set up your database connection in the `.env` file.**

5. **Run database migrations:**
   ```bash
   npm run migrate
   ```

6. **Run the backend server:**
   ```bash
   npm start     # or yarn start
   ```

## Database Setup

1. **Install MySQL/PostgreSQL** if you haven't already.

2. **Create a new database:**
   ```sql
   CREATE DATABASE kigoo_template;
   ```

3. **Import initial data (if available):**
   ```bash
   # Example for MySQL
   mysql -u your_username -p kigoo_template < path/to/initial_data.sql
   ```

## Docker Setup (Optional)

If you prefer using Docker, follow these steps:

1. **Build the Docker container:**
   ```bash
   docker-compose up --build
   ```

2. **Access the application at:**
   ```
   http://localhost:3000
   ```

## Conclusion

You should now have the Kigoo Template up and running on your local machine. For further information, please refer to other documentation files or the repository README.
