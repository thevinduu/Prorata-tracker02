# Semester Command Centre — Pro-Rata Tracker

A lightweight, responsive semester tracker for the 2026/JUL SLIIT pro-rata workload.

## Features

- 8 course dashboards
- Overall completion percentage
- Completed / open / due-soon tracking
- Search and module filters
- One-click CourseWeb / submission links
- Pro-rata GitHub lab links for IT1120
- Personal task creation
- Progress saved in browser `localStorage`
- Works as a static GitHub Pages site — no backend required
- Mobile-friendly layout

## Important limitation

Progress is stored in the browser you use. It is **not synchronized between devices**. If you want the same progress on your phone, laptop, and university PC, the next version should use a small database such as Supabase or Firebase with login.

## Deploy on GitHub Pages

1. Create a new GitHub repository, for example `prorata-tracker`.
2. Upload `index.html` and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder, then save.
6. GitHub will provide your public site URL.

Typical URL format:

`https://YOUR-GITHUB-USERNAME.github.io/prorata-tracker/`

## Editing the tracker

The course data is stored near the top of `index.html` in the `courses` array. You can add, remove, or edit tasks there.

For tasks whose official deadline is not yet published, the tracker intentionally leaves the date blank rather than guessing.
