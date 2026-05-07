# Bond Tracker 🔥

A gamified father & son activity tracker. Log conversations, chores, volunteering, adventures, and more — earn points, build streaks, unlock badges.

## Files in this project

```
bond-tracker/
├── public/
│   └── index.html
├── src/
│   ├── index.js
│   └── App.js
├── package.json
└── README.md
```

---

## How to deploy (step-by-step, no coding experience needed)

### Step 1 — Create a GitHub account
1. Go to **github.com**
2. Click **Sign up** and create a free account
3. Verify your email

### Step 2 — Create a new repository (your project folder online)
1. Once logged in, click the **+** icon in the top right → **New repository**
2. Name it: `bond-tracker`
3. Keep it set to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
1. On your new repository page, click **uploading an existing file**
2. You need to upload the files in the correct folder structure. GitHub lets you drag and drop.
3. Upload all files keeping the folder structure intact:
   - `public/index.html`
   - `src/index.js`
   - `src/App.js`
   - `package.json`
4. Scroll down, click **Commit changes**

### Step 4 — Create a Vercel account
1. Go to **vercel.com**
2. Click **Sign Up** → choose **Continue with GitHub** (this connects them automatically)
3. Authorize Vercel to access your GitHub

### Step 5 — Deploy to Vercel
1. On the Vercel dashboard, click **Add New → Project**
2. You'll see your `bond-tracker` repository listed — click **Import**
3. Vercel will auto-detect it's a React app
4. Click **Deploy** — that's it!
5. In about 60 seconds you'll get a live link like: `bond-tracker.vercel.app`

### Step 6 — Share the link
Send that link to your son. It works on any phone browser — no app download, no account needed.

---

## How data works

Right now each person's data is saved **locally on their own device** (in the browser). This means you each have your own tracker.

To get **shared/synced data** between two phones, ask Claude to add Supabase integration (free database). That upgrade will let both of you see the same logs and points in real time.

---

## Customizing the app

Want to change activity names, point values, or colors? Open `src/App.js` and look for the `CATEGORIES` array near the top. Each item has:
- `label` — the name shown on the button
- `points` — how many points it's worth
- `color` — the highlight color (hex code)
- `icon` — the emoji
- `desc` — the description text

Change any of these and re-upload to GitHub — Vercel will automatically redeploy.
