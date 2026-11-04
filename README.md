# Research Studio public preview

Static HTML/CSS/JavaScript dashboard prepared for GitHub Pages. Publish this directory as the repository root and configure Pages to deploy from the selected branch root. No build or dependency install is required. Relative assets support a project path such as `/research-studio/`.

This is a synthetic preview, not a research service. There are no real participants, accounts, credentials, persistent storage or backend calls. Changes reset on reload. The public build disables the local sign-in/API route. It cannot assign tasks to Android or collect research data. Cognitive tasks are nonvalidated adaptations.

Source: October 24 final ResearchFoundation package, Library version 2. Its researcher-web source was copied, then public-preview wording and an explicit backend-disable guard were added. No Android/backend files, private hosting metadata, credentials or git history are included.

## Publish on GitHub Pages

1. Unzip this archive. Upload its contents (not the ZIP itself) into the root of your GitHub repository. Keep `index.html`, `app.js`, and `style.css` together. Include the hidden `.nojekyll` file if your upload method supports it.
2. Commit the files to your chosen branch, usually `main`.
3. In the repository, open **Settings → Pages**. Choose **Deploy from a branch**, select that branch and **/ (root)**, then save.
4. Wait for GitHub's deployment to finish, then open the URL shown in Pages settings. For a project repository it is usually `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`.

The archive does not create a repository or enable Pages for you. Pages availability depends on your repository visibility and GitHub plan. Keep the deployed files public-preview only; do not add credentials or real study data.

## Try it locally

Open `index.html` in a current browser, or serve this folder using `python3 -m http.server 8000` and open `http://localhost:8000`. Clipboard buttons may require a secure browser context and permission. No package installation or build step is needed.

## Readability update · November 4, 2026

- Short, direct page titles and instructions; repeated task badges and workflow filler removed.
- Larger body and helper text, darker secondary text, clearer spacing and mobile wrapping.
- All 12 cognitive tasks, study selection, enrollment samples, team controls and protocol planning remain available.
- Demo/privacy warnings, reset-on-reload behavior and clinical-validation limitations remain visible.
- Active navigation now exposes `aria-current`; the publish dialog has an accessible name and description. Keyboard focus is restored after task updates.
- Fixed sample invitation feedback disappearing immediately and cleared the dialog result before each review so Escape cannot reuse an earlier publish action.

### Verification

Passed JavaScript syntax checking and mocked-DOM state/render regression checks: selections, publish/discard, empty configuration, dialog result reset, sample enrollment, invitation feedback, disabled backend/sign-in, protocol controls, new studies and per-study configuration.

Full browser interaction and visual checks could not run in the build environment because Chromium was blocked from creating its required local socket. Responsive layout and native keyboard/dialog behavior still need a browser smoke test. This package has not been deployed.
