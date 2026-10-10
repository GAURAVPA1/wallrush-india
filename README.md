# WallRush India — deployment package

## Website
Upload this folder to Netlify, Vercel, or GitHub Pages. Point `wallrush.in` to the hosting provider.

## PWA
`manifest.webmanifest` and `sw.js` make the site installable on supported mobile browsers.

## Online rooms
Edit `firebase-config.js` and set `window.WALLRUSH_FIREBASE_URL` to your Firebase Realtime Database URL. Configure Firebase Realtime Database rules before enabling public rooms; do not put service-account/private credentials in the frontend.

## Android
The `android/` folder is a minimal native WebView wrapper source. Set the production URL in `MainActivity.java`, then build a signed AAB with Android Studio/Gradle for Google Play.
