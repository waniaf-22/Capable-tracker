# Capable: Learning Roadmap Tracker

Static site: plain HTML, CSS and JavaScript in `index.html`. No build step.

## Deploy on Vercel
1. Push this folder to a GitHub repo.
2. In Vercel: Add New → Project → import the repo.
3. Framework preset: **Other**. Leave build command and output directory empty.
4. Deploy.

Or with the CLI from inside this folder: `npx vercel` (then `npx vercel --prod`).

## Use on your phone
Open the Vercel URL, then:
- iPhone (Safari): Share → Add to Home Screen
- Android (Chrome): menu → Add to Home screen / Install app

## Data
Stored in each browser's localStorage, so phone and laptop keep separate data.
Move data between devices with Settings → Export JSON / Import JSON.
All storage goes through `StorageAdapter` / `Repo` near the top of the script, which is the place to swap in Supabase for sync.
