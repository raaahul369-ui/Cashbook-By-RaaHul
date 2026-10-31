# CashBook By RaaHul for Android

An offline-first personal and couple expense tracker starter project.

## Current starter features
- Expense entry: date, amount, category, payer, remarks
- Default payers: Rahul and Suchithra (customisable)
- Manually add, rename, activate/deactivate, and delete categories and payers
- Daily and current-month payer summaries
- All-time payer and category summaries
- CSV export using Android's file picker
- Local SQLite storage; no account or internet connection required
- Default currency AED (editable in Manage)

## Build the APK with GitHub Actions
1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Open **Actions** and run **Build CashBook By RaaHul APK**, or push to `main`.
4. Open the completed workflow run and download the `CashBook-By-RaaHul-debug-apk` artifact.
5. Extract it and install `app-debug.apk` on your Android phone. You may need to allow installation from your file manager/browser.

The workflow builds a debug APK for testing. A signed release APK should be configured before distributing the app publicly.

## Build locally
Requires JDK 17, Android SDK (API 35), and Gradle 8.9:

```bash
gradle assembleDebug
```

APK output: `app/build/outputs/apk/debug/app-debug.apk`.

## Important scope notes
This is a first usable starter, not a finished production finance product. It currently stores one payer per expense and supports CSV export. Cloud synchronisation, multi-payer amount allocation, Excel/PDF export, receipt attachments, backup/restore, charts, and advanced custom date-range reports are not implemented yet. Data is stored locally on the device, so back up the phone before uninstalling the app.
