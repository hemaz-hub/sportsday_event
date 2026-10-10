# College Sports Fest 2026 — Frontend / localStorage edition

A responsive, no-build-step frontend made with HTML, CSS, Bootstrap 5, and JavaScript. It does not require Node.js, Python, npm, or a database server.

## Run it

1. Extract the ZIP.
2. Open `index.html` in your browser, or use VS Code's Live Server extension if available.
3. Internet is needed for the Bootstrap and Google Fonts CDNs and the remote sports photos. The website code itself does not need a build step.

## Included

- Responsive sports-themed homepage and eight separate game cards.
- Game details, rules, venue, assigned date and morning/afternoon session.
- Student registration forms with dynamic team-member fields.
- Team sizes: Cricket 11, Kabaddi 7, Badminton 1, Volleyball 6, Throwball 7, Chess 1, Carrom 1, Basketball 5 (Team Lead included).
- Branch and section options: CSE A–E; IT A–C; AIML A; AIDS A–B; CSC (Cyber Security) A; ECE A–B; EEE A; MECH A–B; CIVIL A.
- Register number validation using exactly `NNLNNLNNNN`, e.g. `25B81A4605`.
- Duplicate same-game registration prevention and within-team duplicate prevention.
- Registration period 8–15 October 2026; event dates 21–25 October 2026; morning 10:30 AM–1:00 PM and afternoon 2:00 PM–4:30 PM.
- Celebration/receipt after registration, print/save as PDF, local admin dashboard, stats and CSV export.

## Important limitations of a frontend-only portal

- Registrations are saved in this portal on the current device using `localStorage`. They do not sync between devices. Clearing this site's stored data can erase them.
- The admin screen is a demonstration only. Demo credentials in `app.js` are `admin` / `sportsfest-demo`; they are visible in source code and are **not secure**. Do not use this version for confidential student data or a real college-wide registration rollout.
- Frontend validation can be bypassed by a technically capable user. Without a server and shared database, it is not possible to guarantee a private admin dashboard, trusted records, or shared college-wide statistics.
- Game dates and sessions are example allocations across the event window and should be confirmed by the college organizer.
- Sports photos are loaded from Unsplash URLs, so internet access is needed for them. Replace the URLs in `app.js` with approved college images as needed.
- This demo blocks submissions outside the stated registration dates based on the device's current clock.
