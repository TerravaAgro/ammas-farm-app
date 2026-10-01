# Amma's Farm: build the Android app (APK) for free on GitHub

GitHub builds the app in the cloud. You don't need Android Studio or a powerful computer.

1. Create a free account at https://github.com and sign in.
2. Click **+** (top right) > **New repository**. Name it `ammas-farm-app`, choose **Private**, click **Create repository**.
3. On the new page click **uploading an existing file**. Unzip this folder on your computer and drag **everything inside it**
   into the page (including the `.github` folder). Click **Commit changes**.
   - On a Mac, the `.github` folder is hidden. If it doesn't upload: click **Add file > Create new file**, type the name
     `.github/workflows/build-android.yml`, paste the contents of `WORKFLOW-COPY-build-android.yml`, and click **Commit changes**.
4. Open the **Actions** tab. A run called "Build Android app" starts by itself and takes about 5 to 8 minutes.
   A green tick means the app is ready.
5. Open the **Releases** page of the repository (right side of the main page) on your Android phone and tap **AmmasFarm.apk**.
6. Tap the downloaded file. Allow "Install unknown apps" for your browser or Files app when asked, then tap **Install**.
   If Play Protect warns about an unknown developer, tap **More details > Install anyway**. That warning appears for every app
   that doesn't come from the Play Store.

To update the app later, replace `www/index.html` in the repository. GitHub builds a new APK automatically.
