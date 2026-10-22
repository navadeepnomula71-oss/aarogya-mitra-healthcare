# Aarogya Mitra – Healthcare MVP (front-end prototype)

Demonstration prototype. All doctors, labs, prices and availability are fictional. Not for real patient data.

## Run
No build step. Open `index.html` in a browser, or serve the folder:

    python3 -m http.server 8000

Then visit http://localhost:8000 (voice input needs localhost or HTTPS).

## Files
- `index.html` – page shell
- `styles.css` – theme, light/dark, high-contrast, assistant styles
- `app.js` – routing, English/Telugu strings, patient/doctor/admin portals, voice assistant

## Features
- Patient/Family, Doctor and Admin portals (doctors stay Pending until an admin approves)
- Family members with separate records, requests, cancel, record download
- Doctor requests (accept/reject/complete + notes), availability slots, double-booking check
- Admin: doctor verification, suspension, stats, audit log
- English/Telugu UI, large text, high contrast
- Voice assistant (Web Speech API, rule-based, confirms before booking/cancelling, 112 emergency message)

## Limits
- Data is stored in browser localStorage only (no backend/SQLite, no shared data between devices)
- Passwords are salted and hashed in the browser: NOT real security
- No email verification, password recovery, real file storage, SMS or AI model
- Next step: Node/Express + database + server-side auth, then a server-side AI intent layer
