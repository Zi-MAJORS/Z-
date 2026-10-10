# JARVIS Android Starter (Free PWA)

This is a beginner-friendly installable web app for Android. It can be added to the home screen and provides:
- Speech recognition when supported by the browser
- Spoken replies using the browser/device text-to-speech engine
- Time and date commands
- Google web searches and website shortcuts
- Optional Gemini API integration for AI answers

## Important limitations
- This is a PWA/web app, not a compiled native APK.
- Microphone speech recognition usually works best in Chrome on Android and may use an online speech service.
- A web app cannot freely control Android apps or protected system settings. Website shortcuts open in the browser.
- If you add an API key, it is stored in browser local storage on that device. Do not publish or share the app with your key. API use may have limits or costs.

## Easiest installation on an Android-only phone
PWA installation requires an HTTPS website. One free method is GitHub Pages:
1. In your browser, sign in or create an account at https://github.com.
2. Create a new public repository, e.g. `my-jarvis`.
3. Upload all files from this folder to the repository root: `index.html`, `manifest.json`, `sw.js`, `icon.svg`.
4. Open repository Settings → Pages.
5. Under Build and deployment, choose Deploy from a branch, select `main` and `/(root)`, then Save.
6. Wait for the Pages URL to appear. Open it in Chrome on Android.
7. Chrome menu (⋮) → Install app or Add to Home screen.

GitHub Pages is public hosting. Never upload an API key or private information to the repository. The key is entered only in the running app and stored in the browser's local storage.

## Use
Tap the microphone, grant microphone permission, then say:
- "What time is it?"
- "Search NDA 1 2027 syllabus"
- "Open YouTube"
- "Open Google"

For AI answers:
1. Visit https://aistudio.google.com/apikey and check current free-tier availability and terms.
2. Create a key if available.
3. In JARVIS, expand AI setup and paste the key. Do not add the key to any source file or GitHub repository.
4. Ask a general question.

## Files
- `index.html`: interface and app logic
- `manifest.json`: installable app metadata
- `sw.js`: basic offline shell cache
- `icon.svg`: app icon
