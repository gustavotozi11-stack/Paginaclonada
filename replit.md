# Hostinger Horizons

## Project Overview

A pre-built React single-page application (landing page) in Portuguese (pt-BR). The site is a product marketing page with WhatsApp integration, YouTube video embed, and e-commerce conversion elements.

## Tech Stack

- **Frontend**: React + Tailwind CSS + React Router v6 (pre-built bundle)
- **Server**: Node.js built-in `http` module (static file server)
- **Runtime**: Node.js 20

## Project Structure

```
/
├── server.js          # Static file server (port 5000)
├── package.json       # Project metadata
├── public/            # Static assets served to browser
│   ├── index.html     # SPA entry point
│   ├── js/
│   │   └── index-8391e72d.js   # React app bundle
│   └── css/
│       └── index-fa760198.css  # Tailwind CSS bundle
└── replit.md          # This file
```

## Running the App

The app is served by `server.js` as a static file server on port 5000 (host `0.0.0.0`).

- **Workflow**: "Start application" runs `node server.js`
- **Port**: 5000
- **Routes**: `/` and `/privacy-policy` (SPA client-side routing, fallback to index.html)

## Deployment

Configured for autoscale deployment with `node server.js`.
