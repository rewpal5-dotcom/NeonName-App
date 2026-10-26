# NeonName — Android APK

`https://neon-name8700.base44.app/` ke liye native Android shell.

**Direct APK download:** https://github.com/rewpal5-dotcom/NeonName-App/releases/latest/download/app-debug.apk

## Kya hai isme

- **Progress bar** — page load hote waqt upar patli bar
- **Back button** — page history mein peeche jaata hai, bahar nahi nikalta
- **Offline screen** — internet na ho to "Retry" button wala saaf screen
- **External links** — `mailto:`, `tel:`, WhatsApp, UPI, ya doosri site ke link phone ke browser/app mein khulte hain
- **Downloads** — site se koi file download ho to Android ke DownloadManager se Downloads folder mein jaati hai
- Cookies aur localStorage on — isliye site ka data save rehta hai
- **Zoom lock** — pinch zoom, double-tap zoom aur left-right panning band; page device width par fix rehta hai (app jaisa feel)
- Koi ads nahi, koi third-party library nahi, sirf `INTERNET` permission

## Build

GitHub Actions se (`.github/workflows/build-apk.yml`) — har build ek release mein APK attach karti hai.

Local:

```bash
./gradlew assembleDebug
# app/build/outputs/apk/debug/app-debug.apk
```

## Note

Ye debug-signed APK hai — direct install ke liye. Play Store ke liye release keystore se signed build chahiye.

## Tech

Java · minSdk 24 · targetSdk 35 · AGP 8.7.3 · Gradle 8.9

## License

MIT
