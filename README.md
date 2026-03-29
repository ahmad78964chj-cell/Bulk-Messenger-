# 💬 WhatsApp Bulk Messenger — Android App

A clean, dark-themed Android app to send WhatsApp messages to multiple contacts automatically using `wa.me` deep links.

---

## 📁 Project Structure

```
WhatsAppBulkMessenger/
├── app/
│   ├── src/main/
│   │   ├── java/com/bulkmessenger/app/
│   │   │   └── MainActivity.java          ← Core logic
│   │   ├── res/
│   │   │   ├── layout/
│   │   │   │   └── activity_main.xml      ← Beautiful dark UI
│   │   │   ├── drawable/
│   │   │   │   └── input_bg.xml           ← Styled input backgrounds
│   │   │   └── values/
│   │   │       ├── styles.xml             ← WhatsApp dark theme
│   │   │       └── strings.xml
│   │   └── AndroidManifest.xml            ← Permissions + queries
│   └── build.gradle
├── build.gradle
├── settings.gradle
└── gradle.properties
```

---

## ✨ Features

| Feature | Details |
|--------|---------|
| 📱 Multiple Numbers | Comma-separated, with country code |
| ✉️ Custom Message | Full multi-line message support |
| ⏱️ Custom Delay | Set delay in milliseconds (min 1000ms) |
| 🛡️ Random Delay | Extra 0–2000ms random delay for account safety |
| ▶️ Start / ⏸️ Pause / ↺ Resume | Full session control |
| 📊 Progress Bar | Live progress tracking |
| 📝 Activity Log | Real-time log of every action |
| 🔗 wa.me Links | Opens WhatsApp chat directly |

---

## 🚀 How to Import in Android Studio

1. Open **Android Studio**
2. Click **File → Open**
3. Navigate to this `WhatsAppBulkMessenger` folder
4. Click **OK**
5. Wait for Gradle sync to finish
6. Click **Run ▶** (connected device or emulator)

---

## 📲 How It Works

1. Enter phone numbers (with country code, comma-separated)
   - Example: `923001234567, 923337654321`
2. Type your message
3. Set delay (default 3000ms = 3 seconds)
4. Tap **START**
5. App opens WhatsApp chat for each number automatically
6. Pause/Resume anytime

---

## ⚠️ Important Notes

- WhatsApp must be installed on the device
- Each number must include country code (no `+` needed, just digits)
- Pakistan example: `923001234567` (92 = country code)
- Minimum delay is 1000ms for safety
- Random delay is added on top of your delay to avoid bans
- App uses `wa.me` links — no WhatsApp API required

---

## 🎨 Theme

- **Dark background**: `#0A0F0D`  
- **WhatsApp green**: `#25D366`  
- **Accent teal**: `#128C7E`  
- **Material Components** for polished buttons and cards

---

## 📋 Requirements

- Android Studio Hedgehog (2023.1) or newer
- Min SDK: 21 (Android 5.0)
- Target SDK: 34 (Android 14)
- Java 8+
