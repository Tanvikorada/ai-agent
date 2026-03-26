# ARIA v2 — Deployment Guide

## Files you have:
- index.html  ← main app
- manifest.json ← makes it installable
- sw.js ← offline support

## Step 1: Get your Claude API Key
1. Go to https://console.anthropic.com
2. Sign up / log in
3. Click "API Keys" → Create Key
4. Copy the key (starts with sk-ant-...)

## Step 2: Add API Key to the code
1. Open index.html in any text editor (Notepad, VS Code, etc.)
2. Find this line near the top of the script section:
   const API_KEY = 'YOUR_CLAUDE_API_KEY_HERE';
3. Replace YOUR_CLAUDE_API_KEY_HERE with your actual key
4. Save the file

## Step 3: Deploy to Netlify (FREE, easiest)
1. Go to https://netlify.com → Sign up free
2. Click "Add new site" → "Deploy manually"
3. Drag your entire aria-v2 FOLDER onto the upload area
4. Done! You get a URL like: https://your-aria.netlify.app

## Step 4: Install as phone app
1. Open the Netlify URL on your Android/iPhone
2. Android: tap the 3-dot menu → "Add to Home Screen"
3. iPhone: tap Share → "Add to Home Screen"
4. ARIA appears on your home screen like a native app!

## Step 5: Enable Push Notifications
1. Open ARIA → go to Automations tab
2. Tap "Enable Notifications"
3. Allow when browser asks
4. You'll get deadline reminders!

## Notes:
- All your data is saved locally on your device
- Works offline (tasks, notes, timer) once installed
- AI features need internet (Claude API calls)
- GitHub tracker uses GitHub's public API (no key needed)
- The Claude API has a free tier with generous limits for personal use
