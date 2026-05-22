# Qwen AI Web App

This repository contains a full‑stack AI web application powered by **Qwen 2.5 Coder**.

- **backend/** – Node.js/Express server handling chat, file upload, and file‑generation.
- **frontend/** – Static HTML/CSS/JS UI (glass‑morphism design).

## Deploy the backend (free)

We use **Railway** (free tier) to host the backend.
1. Sign up at https://railway.app and create a new project.
2. Connect the GitHub repository (or upload a zip).
3. Railway will detect the `package.json` and install dependencies.
4. Set the start command to `npm start` (or leave default). Railway will expose the service on `https://<project>.railway.app`.
5. Add an environment variable `TOKEN_SECRET` (any random string) in the Railway dashboard.
6. Deploy – the service will be publicly reachable.

## Deploy the frontend (static)

The frontend can be hosted on **GitHub Pages** for free.
1. In the GitHub repo, go to **Settings → Pages**.
2. Choose the `frontend/` folder as the source (or use the `gh-pages` branch).
3. Save – GitHub will publish the site at `https://<username>.github.io/<repo>/`.
4. Update the frontend `app.js` endpoint URLs to point to the Railway backend URL (e.g., `https://my-qwen-app.railway.app`).

## Local development

```bash
# clone the repo
git clone <repo-url>
cd my-qwen-web
# install backend deps
npm install
# start backend
npm start
# open frontend in a browser (serve via live‑server or similar)
```

Enjoy your AI‑powered chat and file‑generation web app! 🎉
