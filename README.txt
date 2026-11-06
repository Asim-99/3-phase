3-Phase Energy Meter Android project — cloud APK build

No Android Studio is required. This project includes a GitHub Actions workflow
that builds the APK in GitHub's cloud and makes it available to download.

Steps:
1. Download and extract this ZIP.
2. Sign in to GitHub and create a new EMPTY repository (for example:
   three-phase-energy-meter). Do not add a README or license there.
3. Upload the extracted project files and folders to that repository, keeping
   the .github/workflows/build-apk.yml file and its folder structure.
   If uploading through the website, GitHub's web uploader may not show hidden
   .github folders. If so, create the workflow file in GitHub using
   Add file > Create new file and name it:
   .github/workflows/build-apk.yml
   Paste the contents from the same file in this project.
4. Open the repository's Actions tab. Select "Build Android APK" and click
   "Run workflow" (or wait for the first push build to finish).
5. Open the completed workflow run. Under Artifacts, download
   three-phase-energy-meter-apk. Extract the downloaded artifact ZIP;
   app-debug.apk is the installable app.

The app uses your supplied Firebase endpoint and refreshes every 5 seconds.
The Firebase database must permit the app's read request.
