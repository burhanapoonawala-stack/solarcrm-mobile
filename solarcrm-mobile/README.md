# SolarCRM Mobile — Deploy & Install Guide

## What this is
A mobile web app that syncs with the same Google Sheet as your desktop SolarCRM.
Works on iPhone Safari. Install it to your home screen — it looks and feels like a real app.

---

## STEP 1 — Deploy to Vercel (free, 5 minutes)

### A) Create a free Vercel account
1. Go to **vercel.com** on your MacBook
2. Click **Sign Up** → choose **Continue with GitHub**
3. Create a free GitHub account if you don't have one (github.com)

### B) Upload the app
1. Go to **vercel.com/new**
2. Click **"Browse"** or drag the entire **solarcrm-mobile** folder into the upload area
3. Vercel auto-detects it's a static site — leave all settings as default
4. Click **Deploy**
5. Wait ~30 seconds

### C) Get your URL
After deploying, Vercel gives you a URL like:
`https://solarcrm-mobile-abc123.vercel.app`

**Save this URL** — this is your mobile app address.

---

## STEP 2 — Open on your iPhone

1. Open **Safari** on your iPhone
2. Go to your Vercel URL (e.g. `https://solarcrm-mobile-abc123.vercel.app`)
3. The setup screen will appear

---

## STEP 3 — Connect to Google Sheets on your iPhone

You need two things:

### A) Your Spreadsheet ID
Same one you use in the desktop app.
From the URL: `docs.google.com/spreadsheets/d/`**`THIS_PART`**`/edit`

### B) Your credentials.json contents
1. On your Mac, find your `credentials.json` file (the one you use for the desktop app)
2. Open it with TextEdit (right-click → Open With → TextEdit)
3. Select all (Cmd+A) and copy (Cmd+C)
4. On your iPhone, paste it into the credentials box in the app

Then tap **Connect & Launch →**

---

## STEP 4 — Add to iPhone Home Screen

This makes it feel like a real app:

1. In Safari, tap the **Share button** (box with arrow pointing up, at the bottom)
2. Scroll down and tap **"Add to Home Screen"**
3. Name it **SolarCRM**
4. Tap **Add**

Now SolarCRM appears on your iPhone home screen with its own icon.
Open it just like any other app — no browser bar, full screen.

---

## What works on mobile
- ✅ Dashboard with today's actions and reminders
- ✅ View all leads
- ✅ Add new leads (full form including site visit details)
- ✅ Edit leads
- ✅ Add tasks / next steps with due dates
- ✅ Mark tasks complete
- ✅ Schedule meetings
- ✅ View all meetings
- ✅ KPI cards (active leads, won, pipeline value, kWp)
- ✅ Search and filter leads by status
- ✅ All data syncs live with your Google Sheet
- ✅ Works on iPhone Safari

## What stays on laptop only
- File attachments (PDFs, photos)
- Project Execution tracker (the 6-stage tracker)
- These are complex features that need the desktop app

---

## Syncing between phone and laptop
Both apps read and write to the **same Google Sheet**.
- Add a lead on your phone → instantly visible on your Mac
- Add a task on your Mac → shows up on your phone when you refresh
- No special setup needed — it's automatic

---

## Troubleshooting

**"Connection failed"** → Make sure the credentials JSON is pasted completely (it's long — scroll to check it's all there)

**Data not loading** → Pull down to refresh the page in Safari, or tap the Vercel URL again

**Can't find credentials.json** → It's the file you downloaded from Google Cloud when setting up the desktop app. Same file.
