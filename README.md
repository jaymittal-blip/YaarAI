# YaarAI - Android Build Instructions

## Quick Build (3 steps)

1. Open Android Studio → File → Open → select this folder
2. Let Gradle sync complete (~2 minutes)
3. Build → Generate Signed Bundle/APK → APK → debug → Finish

The APK will be at: `app/build/outputs/apk/debug/app-debug.apk`

## Requirements
- Android Studio Flamingo or newer
- Java 11+
- Android SDK 33

## What's inside
- `app/src/main/assets/index.html` — The full YaarAI prototype (HTML/JS)
- `app/src/main/java/in/yarai/app/MainActivity.java` — WebView wrapper

## Features in Prototype
- 4 AI Personas (Jugadu Jatin, Filmy Fiza, Cricket Chhotu, Foodie Farida)
- Hinglish AI conversations
- Games: Antakshari, Rapid Fire, Cricket Quiz, Bollywood Trivia, KBC Style
- Mood Tracker
- XP & Streak system
