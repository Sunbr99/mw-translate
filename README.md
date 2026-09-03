# MW Translate 🌐⚡

**Retro-Future Language & Code Terminal PWA**

A powerful progressive web app for language translation and code analysis with a retro-futuristic terminal interface. Works completely offline and can be installed on mobile devices.

## ✨ Features

- 🟢 **Offline-First** - All processing happens locally on your device
- 📱 **PWA Ready** - Install as a mobile app (Android, iOS, Web)
- 💻 **Code Analysis** - Detect code type and provide optimization suggestions
- 🎯 **Language Detection** - Automatically identify input language
- 🔒 **Privacy First** - No data sent to servers
- ⚡ **Retro Terminal UI** - Cyberpunk aesthetic with golden accents
- 🐛 **Debug Mode** - Real-time diagnostics and performance monitoring

## 🚀 Quick Start

### Web Version
```bash
npm install
npm start
```
Then open http://localhost:8080 in your browser

### Mobile (Android APK)

#### Prerequisites
- Node.js 16+
- Android SDK
- Java Development Kit (JDK) 11+

#### Build Steps

1. **Install dependencies:**
```bash
npm install
```

2. **Initialize Capacitor:**
```bash
npm run capacitor-init
```

3. **Add Android platform:**
```bash
npm run capacitor-add-android
```

4. **Sync project:**
```bash
npm run capacitor-sync
```

5. **Open in Android Studio:**
```bash
npm run capacitor-open
```

6. **Build APK in Android Studio:**
   - Select: Build → Build Bundle(s) / APK(s) → Build APK(s)
   - Or use command line:
   ```bash
   npm run build-apk
   ```

7. **Find your APK:**
   - Location: `android/app/build/outputs/apk/release/app-release.apk`

## 📁 Project Structure

```
mw-translate/
├── index.html              # Main app interface
├── manifest.json           # PWA manifest
├── service-worker.js       # Offline cache
├── capacitor.config.json   # Capacitor configuration
├── package.json            # Dependencies
├── android/               # Android project (generated)
└── README.md              # This file
```

## 🔧 Configuration

### Capacitor Config (`capacitor.config.json`)
- App ID: `com.mwtranslate.app`
- App Name: `MW Translate`
- Supports mixed content on Android for local resources

### Service Worker
- Caches all assets for offline access
- Updates automatically when app changes
- Works in background

## 🎮 Usage

1. **Enter Text/Code** - Paste content in the INPUT panel
2. **Translate** - Click TRANSLATE button for language analysis
3. **Analyze Code** - Click ANALYZE CODE for syntax & structure review
4. **Debug Mode** - Toggle DEBUG ON/OFF to see system diagnostics
5. **Clear** - Use CLEAR ALL to reset

## 🐛 Debug Mode Features

When Debug Mode is enabled, you'll see:
- Service Worker registration status
- Cache status
- Current platform (Android, iOS, Web, etc.)
- Console logs prefixed with `[MW DEBUG]`

## 📱 Mobile Installation

### Android
1. Build APK using steps above
2. Transfer `.apk` file to Android device
3. Enable "Unknown Sources" in Settings
4. Install APK
5. Launch app

### iOS (via Web)
1. Open PWA in Safari
2. Tap Share → Add to Home Screen
3. Launch from Home Screen

### Web
- No installation needed
- Works in any modern browser
- Install as PWA via browser menu

## 🛠️ Development Commands

```bash
npm start              # Start dev server
npm run dev            # Same as start
npm run build          # Prepare for deployment
npm run capacitor-sync # Sync with Android project
npm run build-apk      # Build release APK
npm run build-apk-debug # Build debug APK
```

## 📦 Dependencies

- **Capacitor** - Native mobile framework
- **Service Workers** - Offline caching
- **Modern CSS** - No framework dependencies

## 🔐 Security & Privacy

- ✅ No external API calls
- ✅ No data collection
- ✅ No analytics tracking
- ✅ All processing local
- ✅ HTTPS-ready

## 🌐 Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Android Browser (Modern)
- Opera 76+

## 📋 Troubleshooting

### APK won't build
- Check Java version: `java -version` (should be 11+)
- Ensure Android SDK is installed
- Update gradle: `cd android && ./gradlew wrapper --gradle-version 8.0`

### Service Worker not installing
- Check browser console (F12)
- Clear cache and reload
- Enable "Show all caches" in DevTools

### App crashes on launch
- Enable Debug Mode
- Check Android logcat: `adb logcat`
- Verify manifest.json is valid

### Offline not working
- Check Network tab in DevTools
- Verify service-worker.js is registered
- Check Application → Manifest

## 📝 License

MIT License - feel free to use and modify

## 🤝 Contributing

Contributions welcome! Feel free to:
- Report bugs
- Suggest features
- Submit PRs
- Improve documentation

## 📞 Support

For issues and questions:
- Check the Debug Mode for diagnostics
- Review browser console logs
- Test in Chrome DevTools

---

**Made with ⚡ and retro-futuristic vibes** 

v1.0.0 - September 2026
