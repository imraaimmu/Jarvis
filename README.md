# Jarvis — Voice Admin

Voice-controlled admin tool for the Kukoo platform (6ammart).

## What it does

- Streams mic audio to Gemini Live API
- Gemini interprets voice commands and calls function declarations
- Each function maps to a Laravel API endpoint on the Kukoo backend
- Gemini speaks the result back

## Stack

- **Frontend:** Single vanilla JS HTML file (`voice-admin.html`)
- **Voice AI:** Gemini Live API (`gemini-2.0-flash-live`) with function calling
- **Backend API:** Laravel (Kukoo admin panel) at `staging.kukoo.in` / `www.kukoo.in`
- **Auth:** `Authorization: Bearer <ADMIN_VOICE_TOKEN>`

## Setup

1. Get a Gemini API key from [aistudio.google.com](https://aistudio.google.com)
2. Open `voice-admin.html` in a browser
3. Enter your Gemini API key and admin voice token
4. Click the mic and start talking

## Backend

API routes live under `/api/admin/voice/*` on the Kukoo admin panel.
See `docs/superpowers/plans/` in the admin panel repo for implementation plans.
