# Moonmad Calendar

A single-page, no-backend RP helper for Ciprian Moonmad characters.

## What it does

- Defaults to today's date in Vermont (`America/New_York`) when the date is within 2026.
- Shows the astronomical moon phase for the selected date.
- Shows the Moonmad personality influence associated with the nearest principal lunar phase.
- Includes pre-full-moon, full-moon, and recovery-day reminders.
- Includes the Blood Moon and Super Moon notes supplied in the Ciprian game material.
- Includes a clickable monthly calendar.
- Supports shareable date links such as `?date=2026-09-26`.
- Includes a compact Moonmad rules reference.
- Uses no external scripts, analytics, database, cookies, or API calls.

## Astronomy data

The 2026 principal phase dates are based on Timeanddate's Burlington, Vermont Moon Phase Calendar:

https://www.timeanddate.com/moon/phases/usa/burlington-vt

The game rules describe Moonmad behavior as applying during the "days surrounding" four principal phases but do not specify a numerical cutoff. This tool assigns each date to the nearest principal phase so every RP date has one clear influence.

## Hosting on GitHub Pages

This site only needs `index.html`.

1. Create a new **public** GitHub repository.
2. Upload `index.html` to the repository root.
3. Open **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose the `main` branch and `/(root)` folder.
6. Save.

GitHub will publish the site at a URL similar to:

`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY-NAME/`

## Updating it later

The phase dates live near the bottom of `index.html` in the JavaScript array named `phaseEvents`. Another year can be added by copying the same format and updating `SUPPORTED_YEAR` or by expanding the code to support multiple years.
