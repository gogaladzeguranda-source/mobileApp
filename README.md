# Glow Routine

A small mobile web app (PWA) for your skincare shelf.

- **Add products from photos**: pick one or many photos and Claude reads each label, filling in the name, brand, type and when to use it. Products Claude isn't sure about are marked *Check details*.
- **Routines build themselves**: morning and evening steps in the right layering order (cleanser → toner → serums → moisturizer → SPF).
- **Evening actives rotate**: retinoid, exfoliating acids and masks go on the nights you pick, and never on the same night.
- **Daily checklist** with progress for each routine.
- **Reminders**: phone notifications at your morning/evening times, plus a calendar file (.ics) with daily alarms that ring even when the app is closed.
- Works offline. Data stays on your phone (Backup / Restore in Reminders tab).

## AI photo reading

- Opened from Claude (the artifact link), photos are read with your Claude account. Claude asks you to allow it the first time.
- Installed on your phone, add a Claude API key from [console.anthropic.com](https://console.anthropic.com) in **Reminders → AI photo reading**. The key stays on your phone and is sent only to Anthropic.
- With no AI, photos are still saved and you type the details yourself.

## Put it on your phone

1. In GitHub: **Settings → Pages → Deploy from a branch → `master` / root → Save**.
2. Open `https://<your-username>.github.io/mobileApp/` on your phone.
3. **iPhone**: Safari → Share → *Add to Home Screen*. **Android**: Chrome → ⋮ → *Install app*.
4. Open the app → **Reminders**. On iPhone, set up two daily reminders in the Reminders app (steps shown in the app). iOS doesn't let web apps send notifications while closed.

No build step: it's plain `index.html`, `sw.js` and `manifest.webmanifest`.
