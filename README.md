# ClearNote AI - Vercel Deployment Guide

This application is fully compatible with Vercel. Follow these steps to deploy:

## 1. Environment Variables
You **must** add the following environment variable in your Vercel project settings:

- `GEMINI_API_KEY`: Your Google Gemini API Key.

## 2. Firebase Configuration
The application uses `firebase-applet-config.json` for its Firebase settings. Ensure this file is included in your repository or configured correctly.

## 3. Deployment Settings
Vercel should automatically detect the Vite configuration. If not, use these settings:

- **Framework Preset**: Vite
- **Build Command**: `npm run build`
- **Output Directory**: `dist`
- **Root Directory**: `./`

## 4. SPA Routing
A `vercel.json` file has been included to handle client-side routing by rewriting all requests to `index.html`.

---
*ClearNote AI • Secure Clinical Documentation System*
