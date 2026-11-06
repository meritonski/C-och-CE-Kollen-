# CEKoll Web

Web version of the Swedish CEKoll study app. It uses the question bank and checklist from CEKoll 1.2.0 and runs as a static site on GitHub Pages.

## Included

- All 292 questions and study cards from the supplied app (254 school items and 38 optional extra questions).
- Question search and filters for category, topic, question bank, favorites, and review.
- Flashcard practice, multiple choice quiz, and a reading mode with the school's answers.
- Study progress, daily count, checklist, original sources, and light/dark themes.
- Responsive layout and local browser storage. No account, backend, package installation, or build is required.

## Publish with GitHub Pages

1. Create a new GitHub repository, for example `cekoll-web`.
2. Upload the contents of this folder to the repository root and commit them to the `main` branch.
3. Open **Settings → Pages** and set **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. GitHub will show the published URL in the Pages settings after deployment.

You can also run it locally by serving this folder with any static file server. Opening `index.html` directly may block the question JSON because browsers restrict local file requests; for example, with Python installed, run `python3 -m http.server 8000` in this folder and open `http://localhost:8000`.

## Data and privacy

No login or backend is used. Progress stays in `localStorage` in the current browser. Clearing site data removes local progress. The app includes the supplied school materials and does not fetch them from a remote service. Fonts are loaded from Google Fonts when online; system fonts are used when those fonts are unavailable.

## Content note

Question wording, answers, checklist items, and reference materials are carried over from the supplied CEKoll 1.2.0 project. Follow the source app's guidance about learning practical vehicle checks with an instructor.
