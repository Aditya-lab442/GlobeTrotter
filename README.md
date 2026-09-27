# GlobeTrotter

GlobeTrotter is a personalized travel-planning platform for creating
multi-city itineraries, discovering destinations and activities, tracking
budgets, and sharing trips.

Odoo x LDCE Hackathon Project

# Link

 https://globetrotter1-kappa.vercel.app/

## Features

- JWT authentication with optional Google OAuth
- Multi-city trip and day-by-day itinerary planning
- City and activity discovery
- Budget and expense tracking
- Calendar and timeline views
- Public, shareable itineraries
- Optional AI recommendations and Cloudinary image uploads
- Admin dashboard

## Technology

- **Client:** React, Vite, React Router, Tailwind CSS
- **Server:** Node.js, Express, Mongoose
- **Database:** MongoDB
- **Authentication:** JWT bearer tokens and Google OAuth 2.0

## Project layout

```text
admin/        React admin dashboard
backend/      Express API, MongoDB models, and database schema
frontend/     React travel-planning application
docs/         Architecture, API, database, and user-flow documentation
```

## Requirements

- Node.js 20.19 or newer
- npm 9 or newer
- MongoDB (local or hosted)

## Setup

Install all workspace dependencies:

```bash
npm install
```

Create environment files from the provided examples:

```bash
cp backend/.env.example backend/.env
cp frontend/.env.example frontend/.env
```

Set a unique `JWT_SECRET` and configure `MONGO_URI` in `backend/.env`.
Set `VITE_API_BASE_URL` in `frontend/.env` if the API is not running at its
default URL. For deployed environments, set `VITE_ADMIN_URL` to the hosted
admin dashboard URL.

Start the API, travel frontend, and admin dashboard together:

```bash
npm run dev
```

Or run them separately:

```bash
npm run server:dev
npm run frontend:dev
npm run admin:dev
```

The travel frontend runs at `http://localhost:5173`, the admin dashboard at
`http://localhost:5174`, and the API at `http://localhost:5000`. The API health
endpoint is `http://localhost:5000/health`.

## Useful commands

```bash
npm run frontend:build
npm run frontend:lint
npm run admin:build
npm run server:test
npm run seed
```

## Documentation

- [API](docs/api.md)
- [Architecture](docs/architecture.md)
- [Database](docs/database.md)
- [User flow](docs/user-flow.md)

## Project links

- [Live application](https://globetrotter1-kappa.vercel.app/)
- [GitHub repository](https://github.com/prtspndy/GlobeTrotter)
- [Project documentation](https://drive.google.com/file/d/1YQrrHda01JDDPAFVZqlq8hNoSbCO4XQH/view?usp=sharing)
- [Project presentation](https://drive.google.com/file/d/1fIUUQwjfTTtcmx2DnytH89_6pMEUyPOk/view?usp=sharing)
- [Demo video](https://youtu.be/QE_F3dc9Q6M)

## License

This project is developed for educational and hackathon purposes.
