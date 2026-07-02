# Scheduling Assistant

A single-page web app for finding dates that work for everyone. Add participants,
mark each person's availability on a calendar, and the app highlights the best
dates for the whole group.

## Features

- Add participants and track each person's availability by date
- Automatic analysis of the best dates for a chosen month
- Optional "business days only" filter
- Light/dark theme toggle
- Import and export data as JSON
- All data is stored locally in your browser (`localStorage`) — no server required

## Usage

Open `index.html` in any modern web browser. That's it — there is no build step
or installation.

To serve it locally instead:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Tech

Built as a single `index.html` file using CDN-hosted libraries:

- [Alpine.js](https://alpinejs.dev/) — reactivity
- [Tailwind CSS](https://tailwindcss.com/) + [daisyUI](https://daisyui.com/) — styling
- [Day.js](https://day.js.org/) — date handling
- [flatpickr](https://flatpickr.js.org/) — date picker
- [Lucide](https://lucide.dev/) — icons

## Data

Your participants and availability are saved automatically to the browser's
`localStorage`. Use the export button to back up your data as JSON, and the
import button to restore it.
