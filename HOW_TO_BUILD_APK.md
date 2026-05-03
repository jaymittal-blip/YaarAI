# YaarAI – How to Build the APK

## Method 1: Android Studio (Recommended, Free)

### Step 1 – Install Android Studio
1. Download from: https://developer.android.com/studio
2. Install it (Windows/Mac/Linux all supported)
3. During setup, let it install the Android SDK automatically

### Step 2 – Open the Project
1. Open Android Studio
2. Click **"Open"** (not "New Project")
3. Select this `YaarAI_Android` folder
4. Wait for Gradle sync to complete (~2–3 minutes, needs internet first time)

### Step 3 – Build the APK
1. In top menu: **Build → Build Bundle(s) / APK(s) → Build APK(s)**
2. Wait ~1 minute
3. A popup says "APK(s) generated" → click **"locate"**
4. Your APK is at: `app/build/outputs/apk/debug/app-debug.apk`

### Step 4 – Install on your Phone
1. Transfer `app-debug.apk` to your Android phone (WhatsApp, Google Drive, USB cable)
2. On your phone: Settings → Security → **Allow install from unknown sources**
3. Open the APK file on your phone → Install
4. Done! YaarAI is now on your phone 🎉

---

## Method 2: Online APK Builder (No PC setup needed)

### Using Appetize.io (just for demo/testing)
1. Go to https://appetize.io
2. Upload the APK to test in browser

### Using GoNative.io or WebViewGold
1. Go to https://gonative.io (free trial)
2. Enter `file:///android_asset/index.html` as the URL
3. Download the generated APK

---

## Minimum Requirements
- Android Studio Flamingo (2022.2.1) or newer
- Java 11 (bundled with Android Studio)
- Android SDK 33 (auto-downloaded)
- ~5GB disk space for Android SDK

## What's Inside the App
- `app/src/main/assets/index.html` — Full YaarAI app (Groq AI powered)
- `app/src/main/java/in/yarai/app/MainActivity.java` — WebView wrapper
- The app uses WebView to render the HTML/JS app natively on Android
- Groq API key is embedded — no internet setup needed beyond the API call

## Troubleshooting
- **Gradle sync fails**: Make sure you have internet connection on first sync
- **Install blocked**: Enable "Unknown sources" in phone Settings → Security
- **App crashes**: Open Chrome DevTools → chrome://inspect to debug WebView
