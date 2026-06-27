# GPS-Based Trip Tracking Dashboard

Production-ready full-stack project for **Manivtha Tours & Travels** to manage bookings, vehicles, drivers, GPS trip tracking, delay alerts, reports, and customer trip visibility.

## Tech Stack

- Frontend: React, Vite, Material UI, React Router, React Hook Form, Axios, Recharts, Leaflet/OpenStreetMap
- Backend: Node.js, Express, JWT, MySQL2, Joi, Jest, Supertest
- Database: MySQL with normalized tables, foreign keys, seed data

## Folder Structure

```text
backend/          Express REST API
frontend/         React dashboard application
database/         MySQL schema, seed data, ER diagram
docs/             API docs, setup guide, report, PPT content, demo script, viva Q&A
```

## Quick Start

1. Create MySQL database and load scripts:

```bash
mysql -u root -p < database/schema.sql
mysql -u root -p manivtha_trips < database/seed.sql
```

2. Configure backend:

```bash
cd backend
cp .env.example .env
npm install
npm run dev
```

3. Configure frontend:

```bash
cd frontend
cp .env.example .env
npm install
npm run dev
```

Default logins:

- Admin: `admin@manivtha.com` / `password123`
- Driver: `driver@manivtha.com` / `password123`
- Customer: `customer@manivtha.com` / `password123`

## Deployment

- Frontend: deploy `frontend` to Vercel with `VITE_API_BASE_URL`.
- Backend: deploy `backend` to Render with MySQL environment variables.
- Database: use PlanetScale, Aiven, AWS RDS, Railway MySQL, or managed MySQL.

See [docs/SETUP_GUIDE.md](docs/SETUP_GUIDE.md) for full setup.
