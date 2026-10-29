# Raj Training Log PWA

A Windows-friendly Progressive Web App for the personalised 9-day training cycle.

## What is included
- Automatic repeating Day 1–9 schedule
- Set logging for kg, reps and RIR
- Previous best-set display
- Workout history and notes
- Progress chart
- Weight, waist, sleep, recovery, steps and VO2 max check-ins
- JSON export/import backup
- Offline cache after the first successful load
- Local browser storage, with no account, advertising or analytics

## Test on Windows using VS Code
1. Extract this ZIP.
2. Open the `RajTrainingPWA` folder in VS Code.
3. Install the **Live Server** extension by Ritwick Dey.
4. Right-click `index.html` and select **Open with Live Server**.
5. Test workout logging and export a backup.

Opening `index.html` directly is not recommended because service workers require a web origin.

## Put it on your iPhone
The app must be hosted on an HTTPS website before Safari can install and run it reliably as a PWA. A simple option is GitHub Pages:

1. Create a GitHub repository and upload these extracted files to the repository root.
2. In the repository, open **Settings > Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the main branch and root folder, then save.
5. Open the generated Pages address in Safari on the iPhone.
6. Tap **Share > Add to Home Screen > Add**.
7. Open **Raj Training** from the Home Screen.

## Data and privacy
Workout data is stored in browser localStorage on that device/browser. It is not uploaded by this app. Use **Plan > Export data** regularly. Clearing Safari website data or deleting the installed web app may remove local records.

## Programme note
This version uses the known nine-day structure and starter exercise list. Review exercises, ordering, warm-ups and working sets before relying on it. Edit the `programme` array near the top of `app.js` to change the plan.

## Health note
This is a workout logger, not medical software. Given the history of prolapsed discs, stop and obtain appropriate assessment for new or worsening pain, weakness, numbness or loss of function.
