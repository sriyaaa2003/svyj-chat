# SVYJ Chat

A browser-based real-time chat app built on Firebase. Users sign up with an email and password, create or join chat rooms, and exchange messages that update live for everyone in the room.

## Features
- Email/password sign-up and login (Firebase Authentication)
- Chat rooms with live message updates (Cloud Firestore listeners)
- Online-user tracking
- Auto-generated avatars (DiceBear)
- Deployable as a static site with Firebase Hosting

## Tech stack
Vanilla JavaScript (ES modules), HTML/CSS, Firebase (Auth, Firestore, Hosting), `serve` for local hosting.

## Project structure
| Path | Purpose |
|------|---------|
| `index.html` | App shell, login/sign-up screen, Firebase initialisation |
| `app.js` | Auth flow, rooms, messages, online-user logic |
| `styles.css` | Styling |
| `firebase-config.js` | Firebase project configuration |
| `firebase.json` | Firebase Hosting configuration |
| `server.js` | Small Socket.IO server, apparently an earlier prototype (the Firebase version does not use it, and its dependencies are not in `package.json`) |
| `aws-config.js` | Placeholder S3 upload helper (unused, values are placeholders) |

## Run locally
```bash
npm install
npm start      # serves the folder with `serve`
```
To use your own backend, create a Firebase project with Authentication (email/password) and Firestore enabled, then replace the values in `firebase-config.js` and the config object in `index.html`.

## Status
Early-stage personal project (April 2025).
