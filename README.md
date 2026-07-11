# NewPad

Find the right place for mom and dad. WITHOUT filling out a SINGLE lead form.

Search independent living, assisted living, memory care facilities and more - powered by real Medicare Care Compare data. No accounts. No sales calls. No spam.

Built by [Mike Gracen](https://github.com/mgracen).

---

## Features

- **Search by zip code** - find facilities within 10, 25, or 50 miles
- **Real Medicare data** - star ratings, inspection history, license status from the U.S. government
- **Filter by care type** - assisted living, independent living, memory care, skilled nursing, in-home care, respite care
- **Filter by budget** - see only what fits your situation
- **Save facilities** - bookmark places that look promising, notes stay on your device
- **Contact directly** - call or visit facility websites yourself, no middleman
- **No accounts** - nothing to sign up for, nothing to log in to
- **No lead forms** - your info is never passed to facilities or anyone else

---

## Stack

| Layer | Service | Cost |
|---|---|---|
| Frontend | GitHub Pages | Free |
| Backend | Railway | Free tier |
| Facility data | Medicare Care Compare API | Free, no key required |
| Data storage | Browser localStorage | Free |

---

## Setup

### 1. Deploy the backend

- Go to [github.com/mgracen/newpad-backend](https://github.com/mgracen/newpad-backend)
- Follow the Railway deploy instructions in that README
- Copy your Railway URL when done

### 2. Configure the frontend

Edit index.html and fill in your Railway URL at the top of the script:

```javascript
const BACKEND = 'https://your-railway-url.up.railway.app';
```

### 3. Deploy to GitHub Pages

- Push to GitHub
- Settings - Pages - Deploy from branch - main
- Your app will be live at https://mgracen.github.io/newpad

---

## Files

```
newpad/
├── index.html     The entire frontend app
└── README.md
```

---

## Data privacy

Your saved facilities and notes are stored entirely in your browser's localStorage. No data is sent to any server. The backend only queries the Medicare Care Compare API and never receives or stores anything about you personally.

---

## Data source

Facility data sourced from the [Medicare Care Compare API](https://www.medicare.gov/care-compare) - the official U.S. government database of care facilities. Free and public.

---

## License

Personal use. Do whatever you want with it.
