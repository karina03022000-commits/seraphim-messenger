SERAPHIM — Gothic messenger MVP (PWA)
======================================

Included:
- Chat list, create contacts, local message history, message search
- Stories (local notes), Friends list, Profile settings
- Export chats as JSON, clear local data
- Mobile installable PWA shell (HTTPS or localhost needed)

Important limitation:
This version stores chats in the browser's local storage. It does NOT send messages to other devices or people yet. Real WhatsApp-style messaging needs a backend, authentication, realtime transport, and push notifications. No secrets/API keys are included.

How to test:
1. Extract the zip.
2. Open index.html in a browser for basic testing.
3. For installation/offline/PWA service worker, serve the folder over HTTPS or localhost.
   Example using Python from this folder: python -m http.server 8080
4. On phone, open your hosted HTTPS URL in Chrome and use browser menu -> Add to Home screen / Install app.

Files:
index.html — app UI + local functionality
manifest.json — installable web app metadata
sw.js — service worker cache
