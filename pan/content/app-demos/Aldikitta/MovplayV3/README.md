<h1 align="center">Movplay</h1></br>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<div class="embed-container">
    <iframe width="640" height="390" 
    src="https://www.youtube.com/embed/fnLSjrqVM3Y" 
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

Movplay app in Jetpack Compose
(https://github.com/Aldikitta/MovplayV3)

The app is designed to explore movies and tv series powered by the TMDB API.

Tech Stack = MVVM, Hilt, Unit Testing, Retrofit, Room, Paging, Navigation, Compose Destinations, Flow

## Why APK is not available?

The app requires a TMDB API key to fetch data from the TMDB API and google-services.json to connect to Firebase.

The APK is not generated using those because it will be consume the TMDB API quota and the Firebase quota of the developer account of mine.

If you want to build the app manually, follow the instructions below.

## Build Instructions

To build the app manually, follow the instructions below:

### Clone the repo

git clone https://github.com/androiddevnotesforks/adn-MovplayV3

### Open the project in Android Studio

Android Studio Flamingo | 2022.2.1 Canary 9

### Add TMDB API Key

Add your TMDB API key in the local.properties file

In app/build.gradle.kts, modify the following line:

```
buildConfigField("String", "TMDB_API_KEY", "\"your_api_key_here\"")
```

Login to TMDB and get your TMDB API key here: https://www.themoviedb.org/settings/api

Replace your_api_key_here with your TMDB API key.

### Add google-services.json

Go to [Firebase Console](https://console.firebase.google.com/) and create a new project.

Select Android as the platform.

Use the package name `com.example.movplayv3`

Download the google-services.json file and add it to the app folder.

### Build the project in Android Studio

Gradle sync should be successful and the project should build successfully.

### Generating APK

To generate the APK, follow the steps below:

Go to Build > Build Bundle(s)/APK(s) > Build APK(s)

### APK location

app/build/outputs/apk/debug/app-debug.apk

## Additional Info 

Code commit: https://github.com/androiddevnotesforks/adn-MovplayV3/tree/36ea169eb76e368215f89384383cf44a17377b8b

Tweet: https://twitter.com/androiddevnotes/status/1619485348014211073