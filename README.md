# Site Visit Form - Deployment Guide

This project is a ready-to-deploy Netlify site with a serverless function that generates a PDF from the filled form (including drawn signatures) and emails it to HR.

---

## Files included
- `index.html` — Frontend form (mobile-friendly with canvas signatures)
- `functions/submit.js` — Netlify Function: builds PDF and sends email
- `functions/package.json` — dependencies for function
- `netlify.toml` — Netlify config

---

## Quick phone-friendly deployment steps (summary)
1. Create a GitHub account (if you don't have one).
2. Create a new repository on GitHub and upload the files (use "Add file" → "Upload files" in mobile web or GitHub app).
3. Create a Netlify account and on Netlify choose "Import from Git" → connect to GitHub → select the repo → Deploy site.
4. In Netlify site settings → Build & deploy → Environment → add required env variables (SMTP_HOST, SMTP_PORT, SMTP_USER, SMTP_PASS, TO_EMAIL).
5. Redeploy site, open the published URL on your phone and test.

Detailed, step-by-step instructions are provided in the deployment guide included in this project's root README (also in this ZIP).
