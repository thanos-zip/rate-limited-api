# REST API with Rate Limiting

> Build a public REST API with authentication, full documentation and abuse protection using Redis.

## What You Will Learn
- How to design and document a REST API properly
- How rate limiting works and why every public API needs it
- How to use Redis for fast in memory data storage
- How to write API documentation

## Tech Stack
- Node.js
- Express
- Redis
- PostgreSQL
- Railway (deployment)

## Getting Started

### Prerequisites
- Node.js 18+ installed
- Redis installed locally or a free Redis Cloud account
- PostgreSQL installed or Railway database

### Installation
```bash
git clone https://github.com/thanos.zip/rate-limited-api
cd rate-limited-api
npm install
cp .env.example .env
# Add your database and Redis connection strings to .env
npm run dev
```

## Project Structure
```
rate-limited-api/
├── src/
│   ├── index.js                    # Server entry point
│   ├── routes/
│   │   └── api.js                  # API routes here
│   ├── controllers/
│   │   └── apiController.js        # Route logic here
│   ├── middleware/
│   │   ├── rateLimiter.js          # Rate limiting logic here
│   │   └── authenticate.js        # API key verification here
│   ├── db/
│   │   └── index.js               # Database connection here
│   └── redis/
│       └── index.js               # Redis connection here
├── .env.example
├── package.json
└── README.md
```

## What To Build
- Design a simple resource — books, movies or products
- Build full CRUD endpoints — GET, POST, PUT, DELETE
- Generate and validate API keys for authentication
- Implement rate limiting with Redis — max 100 requests per hour per key
- Return proper error messages when limit is exceeded
- Write a simple API documentation page in markdown
- Deploy on Railway

## Stretch Goals
- Add different rate limit tiers — free vs premium API keys
- Build a simple dashboard to monitor API usage
- Add request logging to a database

## Resources
- https://redis.io/docs/getting-started/
- https://www.npmjs.com/package/express-rate-limit
- https://railway.app/docs

---
Built for [@thanos.zip](https://instagram.com/thanos.zip) followers.
