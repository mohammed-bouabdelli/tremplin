# Tremplin - Internship & Employment Platform

A modern platform for managing trainees, internship and job opportunities for ISTA Khemisset.

---

## Setup

### Step 1 - Clone Project

```bash
git clone https://github.com/mohammed-bouabdelli/tremplin.git
cd tremplin
code .
```

---

### Step 2 - Install Requirements

Make sure you have the following installed:

- PHP 8.3+
- Composer
- Node.js 20+
- npm
- MySQL 8+

Check if everything is installed:

```bash
php --version
composer --version
node --version
npm --version
mysql --version
```

---

### Step 3 - Create Configuration Files

Backend:

```bash
cd backend
copy .env.example .env
```

Windows PowerShell:

```powershell
Copy-Item .env.example .env
```

Mac/Linux:

```bash
cp .env.example .env
```

Then configure your database and application settings inside:

```text
backend/.env
```

---

### Step 4 - Install Dependencies

Backend:

```bash
cd backend
composer install
php artisan key:generate
```

Frontend:

```bash
cd ../frontend
npm install
```

---

### Step 5 - Setup Database

Create a MySQL database for the project, then update the database configuration in:

```text
backend/.env
```

Run migrations and seed the database:

```bash
cd backend
php artisan migrate --seed
```

---

### Step 6 - Start Everything

Start the backend:

```bash
cd backend
php artisan serve
```

Then open another terminal and start the frontend:

```bash
cd frontend
npm run dev
```

Open your browser and go to:

[http://localhost:5173](http://localhost:5173)

---

## Admin Account

The seeded default administrator account is:

- Email: `admin@example.com`
- Password: `password`

---

## Common Commands

Run backend server:

```bash
cd backend
php artisan serve
```

Run frontend:

```bash
cd frontend
npm run dev
```

Run migrations:

```bash
cd backend
php artisan migrate
```

Run seeders:

```bash
php artisan db:seed
```

Reset database:

```bash
php artisan migrate:fresh --seed
```

Clear Laravel cache:

```bash
php artisan optimize:clear
```

Build frontend for production:

```bash
cd frontend
npm run build
```
