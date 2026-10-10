# SVYJ Chat

A real-time chat web app built on Firebase. Users sign up with email and password, create or join chat rooms and see messages update live.

## What I did
- Email and password sign-up and login with Firebase Authentication.
- Chat rooms with live messages using Cloud Firestore listeners.
- Online-user tracking.
- Auto-generated avatars with DiceBear.
- Deployed it as a static site on Firebase Hosting.

## How it was built

| File | Purpose |
|------|---------|
| `index.html` | app page, login/sign-up screen, Firebase setup |
| `app.js` | login, rooms, messages, online users |
| `styles.css` | styling |
| `firebase-config.js`, `firebase.json` | Firebase project and hosting config |

## Tech stack
JavaScript (ES modules), HTML, CSS, Firebase (Authentication, Firestore, Hosting).
