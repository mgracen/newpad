# A New Pad for Mom & Dad

> Find the right place for mom and dad. WITHOUT filling out a SINGLE lead form.

Search Medicare-certified skilled nursing and rehabilitation facilities near you. No account. No sales calls. No spam. Just results.

Built by [Mike Gracen](https://github.com/mgracen).

---

## What it does

Most senior care search sites work by collecting your contact information and selling it to facilities as a "lead." You fill out a form, and within minutes your phone is ringing with sales calls that don't stop for years.

A New Pad for Mom & Dad works differently. Search freely, see real results from the U.S. government's Medicare Care Compare database, and contact facilities yourself - on your own terms.

---

## Features

- **Search by zip code or city name** - find facilities within 25 miles
- **Real Medicare data** - star ratings, staffing levels, bed capacity from the official U.S. government database
- **No lead forms** - your contact info is never passed to facilities or anyone else
- **No account required** - nothing to sign up for
- **Save facilities** - bookmark places that look promising, notes stay on your device only
- **Contact directly** - call facilities yourself, no middleman
- **Enter key support** - search without clicking the button
- **Title case names** - clean readable facility names, not ALL CAPS

---

## What's covered

| Care type | Source | Status |
|---|---|---|
| Skilled nursing & rehab | Medicare Care Compare API | Live |
| Memory care units | Medicare Care Compare API | Live (flagged where available) |
| Assisted living | Florida AHCA / state databases | Coming soon |
| Independent living | TBD | Coming soon |

---

## Stack

| Layer | Service | Cost |
|---|---|---|
| Frontend | GitHub Pages | Free |
| Backend | Railway | Free tier |
| Facility data | Medicare Care Compare API | Free, no key required |
| Saved facilities | Browser localStorage | Free, stays on device |

---

## Repos

| Repo | Purpose |
|---|---|
| [newpad](https://github.com/mgracen/newpad) | Frontend - single index.html served via GitHub Pages |
| [newpad-backend](https://github.com/mgracen/newpad-backend) | Express backend - queries Medicare Care Compare API |

---

## How it works

1. User enters a zip code or city name
2. Frontend sends search to Railway backend
3. Backend queries Medicare Care Compare API by state
4. Results filtered client-side by zip prefix
5. Facilities returned with name, address, phone, CMS star rating
6. User contacts facilities directly - no data passed to anyone

---

## Data source

All facility data sourced from the [Medicare Care Compare API](https://www.medicare.gov/care-compare) - the official U.S. Centers for Medicare & Medicaid Services database. Free, public, updated monthly. No API key required.

---

## Privacy

- No user accounts
- No email addresses collected
- No location tracking
- Saved facilities stay in your browser only - never uploaded
- Search inputs never stored or shared
- "Contact directly" always shows the facility's own phone number

---

## Roadmap

- [ ] Assisted living facilities via state licensing databases
- [ ] Memory care filter
- [ ] Inspection history detail view
- [ ] Compare facilities side by side
- [ ] Share a facility via link

---

## License

Personal use. Do whatever you want with it.
