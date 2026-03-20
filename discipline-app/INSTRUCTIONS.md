# 📱 Discipline Daily Tracker — Your Personal App

## What You Have
A fully working Progressive Web App (PWA). It runs like a native phone app
straight from your browser — no App Store, no download, no cost.

---

## 🚀 OPTION 1 — Netlify Drop (Easiest, Free, 2 Minutes)

This is the recommended way. Netlify hosts your app for free.

### Steps:
1. Go to **https://app.netlify.com/drop** in your browser
2. You will see a box that says "Drag and drop your site folder here"
3. Open your file manager / Finder on your computer
4. Find the folder called **discipline-app** (the folder you downloaded)
5. Drag the ENTIRE folder and drop it onto that Netlify box
6. Wait about 30 seconds — Netlify gives you a URL like:
   **https://amazing-name-123.netlify.app**
7. That URL IS your app. Share it or bookmark it.

### Install on your iPhone:
1. Open the URL in **Safari** (must be Safari, not Chrome)
2. Tap the **Share button** (the box with arrow pointing up) at the bottom
3. Scroll down and tap **"Add to Home Screen"**
4. Tap **"Add"** in the top right
5. Done! The app icon appears on your home screen like any other app ✅

### Install on Android:
1. Open the URL in **Chrome**
2. Tap the **three dots menu** (top right)
3. Tap **"Add to Home Screen"** or **"Install App"**
4. Tap **"Add"**
5. Done! ✅

---

## 🚀 OPTION 2 — GitHub Pages (Free, Permanent)

Use this if you want a permanent URL you control forever.

### Steps:
1. Create a free account at **https://github.com**
2. Click the **+** button → **New repository**
3. Name it: **discipline-app**
4. Check **"Public"**, click **Create repository**
5. Click **"uploading an existing file"** link
6. Drag ALL files from your discipline-app folder:
   - index.html
   - manifest.json
   - sw.js
   - icons/ folder
7. Click **"Commit changes"**
8. Go to **Settings** → **Pages** (left sidebar)
9. Under "Source" select **main** branch → click **Save**
10. Your app URL will be:
    **https://YOUR-USERNAME.github.io/discipline-app**

---

## 🚀 OPTION 3 — Run Locally (No Internet Needed After Setup)

If you just want to test it on your computer first:

1. Install **VS Code** from https://code.visualstudio.com (free)
2. Install the **"Live Server"** extension in VS Code
3. Open the **discipline-app** folder in VS Code
4. Right-click **index.html** → **"Open with Live Server"**
5. It opens at http://localhost:5500
6. On your phone (same WiFi): go to **http://YOUR-COMPUTER-IP:5500**
   (Find your IP: Mac → System Preferences → Network. Windows → ipconfig)

---

## 📂 Your File Structure

Your downloaded folder should look like this:

```
discipline-app/
├── index.html        ← The entire app (HTML + CSS + JavaScript)
├── manifest.json     ← Makes it installable as an app
├── sw.js             ← Lets it work offline
└── icons/
    ├── icon-192.png  ← App icon (small)
    └── icon-512.png  ← App icon (large)
```

**Important:** All 4 files + the icons folder MUST be uploaded together.
If you upload only index.html, the install feature won't work.

---

## 📱 How To Use The App

### Today Tab (Home)
- Every morning, open the app
- Work through your 7 disciplines one by one
- Tap each task row to mark it done
- **Daily Reflection** → opens a journal modal. Fill it in and tap Save
- **Progress Photo** → opens camera/upload. Take photo and tap Save
- Both journal and photo only check off AFTER you save them
- Track your water intake by tapping the 8 glass buttons
- The ring fills as you complete tasks — green when all 7 are done 🏆

### Journal Tab
- See all your past entries listed by day
- Tap any card to read the full entry with photo, mood, and reflection
- Or tap "+ Entry" to write today's check-in from here

### Journey Tab
- The 75-day grid shows your full progress
- Green = perfect day, Red = missed, Orange = today, Grey = future
- Tap any day to see exactly which tasks were done

### Stats Tab
- Your current streak, best streak, and perfect days
- Overall challenge progress bar
- Per-discipline completion rates
- Tap "Restart Challenge" to start over from Day 1

### Theme Toggle
- The 🌙 / ☀️ switch in the top right of Today tab
- Flips between dark mode (default) and light mode
- Your choice is remembered

---

## 💾 Your Data

All your data (tasks, journal entries, progress photos) is stored
**locally on your phone** using browser localStorage.

This means:
✅ Works completely offline after first load
✅ 100% private — no server, no account needed
✅ Free forever

⚠️ Important: If you clear your browser data or switch phones,
your data will be lost. To protect it:
- Don't clear Safari/Chrome site data for this URL
- Avoid using "private/incognito" mode
- Consider backing up by exporting data (future feature)

---

## 🔧 Want to Customize It?

Open **index.html** in any text editor (Notepad, TextEdit, VS Code).

### Change the task names:
Find this section near the bottom of index.html:
```
var TASKS=[
  {id:'wu', em:'🌅', name:'Wake Up & Morning Routine', ...},
  ...
```
Change the `name` and `em` (emoji) values to whatever you want.

### Change the number of days (not 75):
Search for `75` in the JavaScript and change the values.

### Change the accent color:
Find `--acc:#FF6B1A` near the top and change the hex color.

---

## ❓ Common Questions

**Q: It doesn't show "Add to Home Screen" on iPhone**
A: Make sure you're using Safari (not Chrome or Firefox) on iOS.

**Q: The app asks to access my camera**
A: That's normal — it's for the Progress Photo feature. Tap Allow.

**Q: I accidentally cleared my browser data**
A: Unfortunately data is lost. This is the trade-off of local storage.
   For cloud backup, ask about adding Firebase sync.

**Q: Can I share this with friends?**
A: Yes! Just share your Netlify/GitHub URL. Each person gets their own
   separate data stored on their own device.

**Q: How do I update the app?**
A: Edit index.html, then re-upload it to Netlify or GitHub.
   Netlify: drag and drop again. GitHub: commit the new file.

---

## 🌐 Future Upgrades (When You're Ready)

1. **Cloud sync** — Add Firebase so data backs up and syncs across devices
2. **Push notifications** — Get daily reminders on your phone
3. **App Store** — Package with Capacitor and submit to Apple/Google
4. **Share progress** — Auto-generate a shareable daily summary image

---

Built with love. Go build discipline. 🔥
