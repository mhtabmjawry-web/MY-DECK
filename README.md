# ReCardo

An installable flashcard Progressive Web App packaged from the original ReCardo HTML app.

## Features
- Original flashcard decks, folders, and spaced-repetition flow.
- Sentence-by-sentence answer review and rating.
- IndexedDB storage for cards, progress, and settings.
- HTML/JSON import and JSON backup/restore.
- Green-blue lightning app icon.
- Web app manifest and service worker for offline app-shell access.
- GitHub Actions deployment workflow for GitHub Pages.

## GitHub Pages
The workflow in `.github/workflows/deploy-pages.yml` deploys the repository root when pushed to `main`. If Pages is not enabled automatically, choose **Settings → Pages → Build and deployment → Source → GitHub Actions**.

## Android installation
Open the HTTPS Pages address in Chrome, let the first load finish, then choose **Install app** or **Add to Home screen**.

## Local data
The app keeps cards and progress in IndexedDB under `flashcards_db_v1`. Data is local to the browser origin and device. Moving from a local HTML file or another site to the new Pages domain creates a separate storage area; use **Back up** in the old app and **Restore** in the new one to transfer existing cards.
