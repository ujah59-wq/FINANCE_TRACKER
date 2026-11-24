MONEY TRACKER - DEPLOYMENT GUIDE (GitHub + Vercel)
===================================================

WHAT YOU HAVE
- index.html  = the whole app (one self-contained file, no build step)
- README.txt  = this guide

STEP 1 - PUT THE APP ON GITHUB
1. Sign in (or sign up free) at https://github.com
2. Click "+" (top right) > "New repository".
3. Name it e.g. money-tracker. Choose Private or Public. Click "Create repository".
4. On the new repo page click "uploading an existing file".
5. Drag in index.html and README.txt. IMPORTANT: index.html must sit in the
   top level of the repo (not inside a folder).
6. Click "Commit changes".

STEP 2 - DEPLOY WITH VERCEL
1. Go to https://vercel.com and choose "Sign Up" > "Continue with GitHub".
2. Click "Add New..." > "Project".
3. Find your money-tracker repo and click "Import" (grant access if asked).
4. Settings: Framework Preset = "Other". Leave Build Command and
   Output Directory EMPTY. Root Directory = ./
5. Click "Deploy". After about a minute you get a link like
   https://money-tracker-xxxx.vercel.app

STEP 3 - INSTALL ON YOUR IPHONE
1. Open the Vercel link in Safari.
2. Tap Share > "Add to Home Screen" > Add.
It then opens full screen like an app.

UPDATING THE APP LATER
- In GitHub open index.html > pencil icon (or Add file > Upload files to
  replace it) > Commit. Vercel redeploys automatically.

IMPORTANT NOTES
- Your data (income, months, pictures, settings) is saved in the browser on the
  device you use (localStorage). It does NOT sync between devices, and clearing
  Safari website data will erase it. Use the same Home Screen icon each time.
- Vercel's free "Hobby" plan is enough for this app.
- Optional: In Vercel > Project > Settings > Domains you can add your own
  domain name.

FEATURES ADDED IN THIS VERSION
- Two financial timelines (switch on the Summary page): Oct - Dec 2026, then
  Jan - Dec 2027. Month pages, calendar and totals follow the chosen timeline.
- Backup: Settings > Backup lets you Export your profile to a .json file (or
  copy it) and Import it on another device or browser. Importing replaces the
  data on the device. Export regularly as a safety copy.
- Pinch-zoom is disabled so it behaves like an app.

VERSION 2 NOTES
- Older exported profiles can be imported into newer versions. Anything that
  the older file did not contain is filled with defaults, and a notice is
  listed under Settings > Import notices (each can be cleared).
- New: shift start/finish times (hours calculated automatically), shift costs
  (shown as "Shift Costs" under Expenses on the Month page), income pay dates
  (received vs expected), and a savings goal meter on the Summary page.

VERSION 3 NOTES
- Summary page: each section heading is now a drop-down (tap to open/close).
  The calendar stays open and sits above "Average income per month".
- Month page: the "Shift Costs" actual now equals its budget.
- Settings > "Notes for Update": a notepad for changes you want next.

VERSION 4 NOTES
- Month page: you can enter a "Budgeted income" for the month, so Budget and
  Actual income in the Overview can differ (blank = use projected pay).

VERSION 5 NOTES
- Actual income now uses the tax rate of the month's full gross pay (ticking
  only some shifts no longer drops you into a lower tax band).
- Month page: optional "Actual income received" box to type the real amount.

VERSION 6 NOTES
- Shift costs from one month now show as "Shift Costs" in the NEXT month's expenses.
- Full-time streams have an optional start month and end month.
- Full-time = 8h Mon-Fri (40h/week); shown on the Summary calendar (hollow dots)
  and counted in the stream's hours.

VERSION 7 NOTES
- Shift costs of a month now appear in the PREVIOUS month's expenses (e.g. November shift costs show under October Shift Costs).

VERSION 8 NOTES
- Month page "Shift Costs" = costs of the NEXT month income stream shifts (using each stream pay period/cut-off), e.g. November shows December shift costs.

VERSION 9 NOTES
- Part-time streams have a "Usual cut-off day". Pay periods run from the day after the previous cut-off to this cut-off (e.g. 21 Nov - 20 Dec = December pay). Month page "Shift Costs" for November = costs of shifts in the December pay period.

VERSION 10 NOTES
- Part-time streams: set an explicit Pay period start and end date for each month. The Month page Shift Costs row shows the date range it is counting (next pay period).

VERSION 11 NOTES
- New streams and shifts start blank (no preset rate, pay day, shift times or hours). Settings > Clear all data wipes everything on the device.

VERSION 12 NOTES
- Settings > Backup: "Share backup" opens the iPhone share sheet (AirDrop, Mail, Messages, Files).

VERSION 13 NOTES
- Settings > Appearance > Layout: Mobile view or Website view. Website view is wider, uses two columns on large screens, has the menu at the top and no drop-down sections.

VERSION 14 NOTES
- Full-time net pay = monthly salary - (salary x 0.041) - 50.20 - 61.58.

VERSION 15 NOTES
- Month page > Expenses: Rent row repeats on following months; changing it in a month updates that month and all later months.
- Backups are named like "22-11-2026 (14-30).json".
- Summary: Projected savings by the end of the timeline, based on your average monthly saving.

VERSION 16 NOTES
- Undo button (top right): up to 4 steps back, shows which section was undone and jumps to that page.
- Full-time streams: salary increases (effective from a month, earlier months unchanged) and pre-tax costs taken from gross monthly pay before the net calculation.

VERSION 17 NOTES
- Website view now uses layout B: a top bar (name, tabs, undo, settings), a stats strip, a wide calendar on the left and graph/projection/lists on the right.

VERSION 18 NOTES
- Website view has a left sidebar (Summary, Income, Month, timelines). Undo and redo are symbol buttons (up to 4 steps each).
- Time, date and month fields now only save when you tap off the field or press the tick button next to it.
- The gear button now reads "Settings".
