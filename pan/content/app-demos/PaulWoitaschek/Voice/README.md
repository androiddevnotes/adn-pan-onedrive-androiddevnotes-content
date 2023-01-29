<h1 align="center">Voice</h1></br>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<div class="embed-container">
    <iframe width="640" height="390" 
    src="https://www.youtube.com/embed/o1vZmO0ydS8" 
    frameborder="0" allowfullscreen></iframe>
</div>
<style>
.embed-container {
  position: relative;
  padding-bottom: 56.25%;
  height: 0;
  overflow: hidden;
  max-width: 100%;
}
.embed-container iframe,
.embed-container object,
.embed-container embed {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>
<br>

## About

Voice app in Jetpack Compose
(https://github.com/PaulWoitaschek/Voice)

The app is a minimal audiobook player using ExoPlayer.

Tech Stack = MVVM, Unit, UI Testing, Room, DataStore, FFmpeg, Material, ExoPlayer, Flow

## APK

APK is available to download in the [assets](assets) directory.

Install APK on your device and open the app.

## Build Instructions

To build the app manually, follow the instructions below:

### Clone the repo

git clone https://github.com/androiddevnotesforks/adn-Voice

### Open the project in Android Studio

Android Studio Flamingo | 2022.2.1 Canary 9

### Build the project in Android Studio

Gradle sync should be successful and the project should build successfully.

### Generating APK

Open terminal and run the following command from the project root directory:

```
./gradlew assembleDebug -x test
```

### APK location

app/build/outputs/apk/debug/app-debug.apk

## Additional Info 

Code commit used to generate APK: https://github.com/androiddevnotesforks/adn-Voice/tree/c285d03c58cacc69153c4989c93ce7e0ea435374

Tweet: https://twitter.com/androiddevnotes/status/1619109000942964738