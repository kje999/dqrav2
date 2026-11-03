# DQRA — Disaster Quick Response App (Official Release Distribution)

Official public release repository for the **DQRA (Disaster Quick Response App)** mobile application.

This repository serves strictly as the verified public distribution endpoint for pre-compiled Android APK binaries and release verification checksums. Application source code, private configurations, and administrative backend services are maintained within private municipal infrastructure.

---

## 📲 Download & Web Portal

* **Official Landing Page & Web Portal:** [https://dqra-eaadb-sg-2026-1028.web.app](https://dqra-eaadb-sg-2026-1028.web.app)
* **Direct Latest APK Download:** [https://dqra-eaadb-sg-2026-1028.web.app/download](https://dqra-eaadb-sg-2026-1028.web.app/download)
* **GitHub Releases Archive:** [https://github.com/kje999/dqrav2/releases](https://github.com/kje999/dqrav2/releases)

---

## 🛡️ System Compatibility & Requirements

* **Operating System:** Android 8.0 (Oreo) through Android 15
* **Package Size:** 163.5 MB (universal APK)
* **Architecture:** Universal Android (ARM64-v8a, armeabi-v7a, x86_64)
* **Required Permissions:**
  * Location (Fine / Coarse) — for incident reporting and station proximity mapping
  * Notifications & Alarms — for high-priority emergency sirens and dispatch alerts
  * Internet — for Firestore live synchronization (with offline incident caching fallback)

---

## 📦 How to Install (Android Sideloading)

1. Download `dqra-app.apk` from the [Releases tab](https://github.com/kje999/dqrav2/releases) or the landing page above.
2. If Chrome displays *"File might be harmful"*, select **Download anyway**.
3. Open the downloaded `.apk` file from your notification tray or Downloads folder.
4. If prompted with *"For your security, your phone is not allowed to install unknown apps from this source"*, tap **Settings** and toggle **Allow from this source**.
5. Tap **Install**, then launch DQRA and grant Location and Notification permissions.

---

## 🔐 Cryptographic Verification

To verify that your downloaded binary matches the official release:

### PowerShell (Windows)
```powershell
Get-FileHash -Algorithm SHA256 dqra-app.apk
```

### Bash (Linux / macOS / Android Termux)
```bash
sha256sum dqra-app.apk
```

Compare the output hash against the `SHA256SUMS.txt` asset attached to each GitHub Release.

---

## 🚨 Municipal Incident Coordination
Developed for integrated response coordination between:
* **Bureau of Fire Protection (BFP)**
* **Municipal Disaster Risk Reduction and Management Office (MDRRMO)**
* Local Government and Barangay Response Units

