# STILL · A personal philosophy practice

A mobile-friendly, single-page web app. It includes daily philosophy reading, reflections, “What challenged me?” with both choices and a free-text option, open-ended daily journaling, a visual jar of good things with saved sticky-note memories and random revisits, experiments in living, future-self letters, My Philosophy, a starter library, saved ideas, progress check-ins, monthly reviews, and JSON backup.

## Run locally
Open `index.html` in a modern browser.

## Publish on GitHub Pages
1. Create a GitHub repository (for example `still-philosophy`).
2. Upload `index.html` to the repository root.
3. Open repository Settings → Pages.
4. Choose deploy from the `main` branch and `/ (root)`.
5. Open the URL GitHub provides.

## Data and cross-device sync
The first version saves data in the current browser's local storage. The same website opens on phone and laptop, but journal entries do not automatically sync yet. In Settings, choose Export my data on one device, transfer the JSON backup privately, and Import backup on the other. Do not commit personal journal exports to a public repository.

For true cross-device sync, add a backend such as Supabase with email authentication and a private per-user data table protected by row-level security. The current build does not pretend sync is enabled. Use only a public anon key in frontend code, never a service-role key. Configure and test authentication, per-user access policies, loading/saving, conflict handling, and recovery before storing private writing.

## Content integrity
The starter library distinguishes paraphrases and summaries from direct quotations where possible. Translations vary. Check linked sources and editions before treating a passage as exact wording. The app is for education and reflection, not diagnosis or treatment.
