# Podcast Transcriber — Starter

This is a minimal Next.js starter that demonstrates:
- Accepting a YouTube link on the frontend
- Server-side download of audio using `ytdl-core`
- Transcribing using OpenAI Whisper via the OpenAI Node SDK

**Important:** This is a starter template. Speaker diarization is NOT included here (you'll need a separate diarization tool like `pyannote.audio` in Python or an external service). This repo focuses on showing the full flow so you can run and deploy a working prototype.

## Setup (locally)
1. Install Node.js (v18+ recommended).
2. Copy `.env.example` to `.env.local` and add your `OPENAI_API_KEY`.
3. Install deps:
   ```bash
   npm install
   ```
4. Run dev server:
   ```bash
   npm run dev
   ```
5. Open http://localhost:3000

## Deploy to Vercel (to get a live link)
1. Push this project to GitHub.
2. Create a new project on Vercel and connect the GitHub repo.
3. Add environment variable `OPENAI_API_KEY` in Vercel settings.
4. Deploy — Vercel will give you a live URL (your public link).

## Notes & Next steps
- Add speaker diarization: use a Python service with `pyannote.audio` or cloud-based diarization.
- Improve UI to match Apple.com styling (this uses Tailwind as a base).
- Add authentication, rate-limiting, and storage for produced transcripts.
