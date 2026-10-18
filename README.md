# Medicine Tracker

A simple Android app for keeping track of your medicines: when you last took each one, when the next dose is due, and reminders so you don't forget. Built with Kotlin and Jetpack Compose, using Material You so the app's colours follow your Pixel's wallpaper.

**Status:** starter app. It opens to an empty "No medicines yet" screen. Adding medicines, reminders and Play Store prep come next.

## What's in here

| Path | What it is |
| --- | --- |
| `app/src/main/java/.../MainActivity.kt` | The app's code. The screen you see is the `HomeScreen` function. |
| `app/src/main/java/.../ui/theme/` | Colours, text styles and the Material You theme. |
| `app/src/main/res/` | Resources: the app name, the launcher icon. |
| `app/build.gradle.kts` | App settings: its ID, version, which Android versions it supports. |
| `gradle/libs.versions.toml` | The libraries the app uses and their versions. |

## Running it on your Pixel

You only need to do steps 1 to 3 once.

### 1. Install Android Studio

Download it from https://developer.android.com/studio and install it with the default options. The first launch runs a setup wizard; pick **Standard** and let it download the Android SDK. This takes a while.

### 2. Get the code

1. In Android Studio's welcome screen, click **Clone Repository** (or **File > New > Project from Version Control** if a project is already open).
2. Paste `https://github.com/spikeisms/medicine-tracker.git` as the URL and click **Clone**. If it asks you to sign in to GitHub, do so.
3. When it asks whether to trust the project, click **Trust Project**.

Android Studio now "syncs" the project, downloading everything it needs. Watch the progress bar at the bottom; wait until it finishes. If it offers to upgrade the Android Gradle Plugin or other versions, it's fine to accept.

### 3. Set up your Pixel for development

1. On the phone, open **Settings > About phone** and tap **Build number** seven times. You'll see "You are now a developer!".
2. Go to **Settings > System > Developer options** and turn on **USB debugging**.
3. Plug the phone into your computer with a USB cable. On the phone, tap **Allow** when it asks to allow USB debugging (tick "Always allow from this computer").

Wireless works too: in Developer options turn on **Wireless debugging**, then in Android Studio use the device menu at the top and choose **Pair Devices Using Wi-Fi**.

### 4. Run the app

1. At the top of Android Studio, check your Pixel is selected in the device dropdown.
2. Click the green **Run** ▶ button (or press Shift+F10 on Windows/Linux, Ctrl+R on Mac).

The app installs and opens on your phone. Change your wallpaper and reopen the app to see the colours follow it.

No phone handy? Use the device dropdown's **Device Manager** to create a virtual Pixel (an emulator) and run on that instead.

## Making a change

Try it: open `MainActivity.kt`, find `"No medicines yet"`, change the text, and press Run again. You can also see the screen without a phone: with `MainActivity.kt` open, click **Split** in the top right to show the preview.

## Automatic builds

Every push to GitHub builds the app automatically (see the **Actions** tab on GitHub). A green tick means it built fine, and each run has a downloadable debug APK.
