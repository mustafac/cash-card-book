# Cash and Card Book: install on your iPhone

The app is 7 small files (plus this guide). You put them on a free website host once, then add that page to your iPhone Home Screen. Your entries are stored on the phone only.

## Step 1. Put the files online (do this on a computer)

Use ONE of these. Menu names may differ slightly from what is written here.

**A. Netlify Drop (quickest)**
1. Go to app.netlify.com/drop.
2. Drag the whole `cash-card-book-app` folder onto the page.
3. Copy the web address it gives you. Create a free Netlify account and claim the site so it is not deleted later.

**B. GitHub Pages (permanent and free)**
1. Create a free account at github.com and make a new public repository, for example `cash-card-book`.
2. Choose "uploading an existing file" and drag in the 7 app files from inside the folder (not the folder itself). Commit.
3. Open Settings, then Pages. Set the source to the main branch, root folder, and save.
4. After a minute or two your address is `https://YOUR-USERNAME.github.io/cash-card-book/`.

The address is public, but the app files hold none of your data. Anyone who opens the link sees an empty app.

## Step 2. Install it on the iPhone

1. Open your address in **Safari** (not inside another app).
2. Tap the Share button, then **Add to Home Screen**, then **Add**.
3. Open the app from its new icon. It works offline after the first load.

## Step 3. Load your existing entries

1. Get `cash-card-book-my-data.json` onto the phone (AirDrop, iCloud Drive or email it to yourself).
2. Open the app **from the Home Screen icon**. An installed app keeps its own storage, separate from Safari.
3. Go to Ledger, then Data, then **Restore from backup file**. Choose the file and tap **Replace everything**.

You should see cash in hand of ₹24,857.00, VISA ₹2,536.04 and RuPay ₹1,784.25.

## Looking after your data

- Entries live only on this phone. Deleting the app or clearing website data erases them.
- Use Ledger, then Data, then **Save backup file** regularly and keep the file in iCloud Drive.
- **Export CSV for Excel** gives you a spreadsheet copy of every entry.
- To update the app later, replace the files on your host and change `VERSION` in `sw.js` (for example to `ccb-v2`).
