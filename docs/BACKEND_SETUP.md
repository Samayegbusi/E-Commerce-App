# Backend Setup Guide

## Prerequisites

- Node.js v18+
- Firebase CLI: `npm install -g firebase-tools`
- Firebase project on Console

## Installation

```bash
cd apps/backend
npm install
firebase login
firebase use --add
cp .env.example .env
# Fill in .env with credentials
```

## Running Locally

```bash
npm run serve
```

## Deploying

```bash
npm run deploy
```

## Database Schema

### Users
```
users/{userId}
├── email
├── displayName
└── createdAt
```

### Products
```
products/{productId}
├── name
├── price
├── stock
└── category
```

### Orders
```
orders/{orderId}
├── userId
├── items
├── total
└── status
```
