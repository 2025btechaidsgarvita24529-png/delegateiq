# DelegateIQ — Web App

AI-powered MUN platform with glassmorphism design, Firebase auth, and badge system.

## Project Structure

```
delegateiq/
├── index.html              ← Landing page
├── css/
│   └── style.css           ← Full glassmorphism design system
├── js/
│   ├── firebase.js         ← Firebase config + auth + badge logic
│   └── app.js              ← Shared app utilities
└── pages/
    ├── login.html           ← Sign in (Firebase Email + Google)
    ├── signup.html          ← Sign up (creates Firestore profile)
    ├── dashboard.html       ← App home (real user data from Firebase)
    ├── ai-chat.html         ← AI Assistant (expandable answers + copy)
    ├── research.html        ← Research tools (5 dedicated tools)
    └── profile.html         ← Profile + badge system (real from Firebase)
```

## How to Run

1. Open in VS Code
2. Install **Live Server** extension
3. Right-click `index.html` → **Open with Live Server**

> ⚠️ Firebase uses ES Modules — must be served via Live Server (not opened as a file://)

## Firebase Setup (already done)

- Project: `delegate-iq-2025`
- Auth: Email/Password + Google enabled
- Firestore: Used for user profiles and badge tracking

## Badge System

Badges are earned automatically:

| Badge | Trigger |
|-------|---------|
| 🚀 First Step | Account created |
| 🏛️ Delegate | First conference added |
| ⭐ Seasoned | 5 conferences added |
| 🔍 Researcher | First AI research query |
| 🎓 Scholar | 10 research queries |
| 📄 Paper Writer | Position paper built |
| 🏆 Award Winner | Award logged |
| 📜 Drafter | Resolution drafted |
| 👥 Committee Member | Committee joined |

## Research Tools

- **Research Bot** → AI chat with expandable answers
- **POO Guide** → Points of Order quick reference
- **Dirt Finder** → Find contradictions in country positions
- **Position Paper Builder** → AI-assisted paper generator
- **Resolution Drafter** → AI clause builder

## USP vs Other Apps

| Feature | Other Apps | DelegateIQ |
|---------|-----------|-----------|
| Answer depth | One-liners | Expandable with full detail |
| Copy responses | ❌ | ✅ One-tap |
| Source citations | ❌ | ✅ Every answer |
| Badge system | ❌ | ✅ Real achievements |
| Research tools | Basic | 5 dedicated tools |
| Auth | Demo only | Real Firebase |

## To Deploy on Netlify

1. Drag the `delegateiq` folder to netlify.com
2. Done — Firebase handles all backend!
