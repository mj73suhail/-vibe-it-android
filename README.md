# vibe.it Android starter

This is a phone-friendly starter project for the vibe.it music discovery app.

## Included
- Dark music-app design
- Search links to official YouTube Music and Spotify services
- Local Liked Songs and user-created playlists saved on the device
- Android project configuration and GitHub Actions workflow to build a debug APK

## Important streaming limitations
This starter does not stream or download copyrighted audio itself. Search results open official music services. It does not automatically import a Spotify account's Liked Songs or playlists. Spotify API playback has account, developer-app, and platform restrictions; Spotify Web Playback SDK streaming requires Premium. See https://developer.spotify.com/documentation/web-playback-sdk/reference and https://developer.spotify.com/documentation/web-api.

## Build APK using only an Android phone
1. Download and extract this ZIP in your phone's Files app.
2. Sign in to GitHub and create a new **public** repository named `vibe-it-android`.
3. On the repository page, use **Add file → Upload files**. Upload the extracted project files and folders, including the hidden `.github` folder if GitHub's mobile upload interface permits it. Commit to `main`.
4. Open the repository's **Actions** tab. Select **Build vibe.it APK**, then **Run workflow** if it has not started automatically.
5. Wait for the workflow to finish successfully. Open that workflow run, scroll to **Artifacts**, and download `vibe-it-debug-apk`.
6. Extract the downloaded artifact ZIP. Tap `app-debug.apk` to install it. Android may ask you to allow your browser or Files app to install unknown apps; only proceed if you trust the build you triggered.

If GitHub's mobile upload interface does not preserve the `.github/workflows/build-apk.yml` path, use GitHub's browser in desktop mode or upload via a Git client. Keep the workflow file in exactly `.github/workflows/build-apk.yml`.

## Notes
- This creates a debug APK for personal testing, not a Play Store release.
- APK building depends on GitHub Actions availability and workflow success.
- The first build may take several minutes.
