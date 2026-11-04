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
