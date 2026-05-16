# React Website

A React application with an Express backend, deployable to Heroku. Previously deployed as a full-stack web application.

## Tech Stack

- React 18
- Express (Node.js backend via `server.js`)
- Heroku deployment

## Setup

```bash
npm install
```

## Running

```bash
./run.sh
```

Or start the Express server directly:

```bash
node server.js
```

## Build

```bash
npm run build
```

## Deployment (Heroku)

```bash
heroku create
git push heroku main
```

View logs:

```bash
heroku logs --tail
```

If you encounter memory issues on Heroku:

```bash
heroku config:set NODE_OPTIONS="--max_old_space_size=2560"
```

Check environment:

```bash
heroku run printenv
```
