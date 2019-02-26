## <p align="center">ANDROID SPLASH SCREEN<p>

## DESCRIPTION

This is and easy to use Splashscreen for android with rotation added that allows you to set time taken to rotate to and direction!

<p align="center">
<img width="250" src="https://user-images.githubusercontent.com/36197725/49332791-9a8b0f80-f5c4-11e8-86b5-fa2171734d7b.gif" alt="Demo!" />
<p>


## LIBRARIES TO NOTE.

1. **[Picasso](https://github.com/square/okhttp)**

- Picasso was used to display the image logo.

- **Picasso** is an image library for **Android**.It caters to image loading and processing. It simplifies the process of displaying images from external locations


2. **[ButterKnife](http://jakewharton.github.io/butterknife/)**

- **Android Butterknife** is a **view binding tool** that uses annotations to **generate boilerplate code** for us.

## THINKS TO NOTE WHILE INTEGRATING!

1. Include the appropriate dependency (or dependencies) listed below in your `app/build.gradle` file.



2. Add The **Main Activity** and **Splashscreen** classes to your project with their xml layouts **activity_main.xml** & **activity_splash_screen.xml**.

- Note that for annimations to work the contents must be inside a Linear Layout.

3. Add animations using the **anim** folder which contains **downtoup.xml** & **uptodown.xml**.

- From this files you can control the **animation setting**.

- You can also set the **duration** as demonstrated below.

```
<?xml version="1.0" encoding="utf-8"?>
<set xmlns:android="http://schemas.android.com/apk/res/android">
    <translate android:toYDelta="0%p"
        android:fromYDelta="100%p"
        android:duration="3000"/>

</set>
```
4. On the **Android Manifest** set the order of loading of activities to **start with Splash Screen**.

```
        <activity android:name=".SplashScreen">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
        <activity android:name=".MainActivity"></activity>
```

- This Will cause the **splash screen** to be load first as the **application launches**. 

5. Depending on the the **Theme** you are using you may want to remove the Action Bar from the Splash Screen just incase your app Theme is set to have an **Action Bar**

- Use whichever seems best to you as for this Demo changes were made in the `app/src/main/res/values/style.xml`

### Splash Page.

<p align="center">
<img align="centre" width="250" src="Spec.md/Disp1.png" alt="Splash page" />
<p>

## PRE-REQUISITES.

A couple of things to get you started:

1. Ensure you have [Java](https://java.com/en/download/) installed

A simple way to install Java is using [sdkman](https://sdkman.io/).

Simply follow the instructions to have _sdkman_ installed and install java:

```bash
sdk install java
```

2. [Gradle](https://gradle.org/)

Gradle is used as the build tool and can be installed with sdkman:

```bash
sdk install gradle
```

3. [Android SDK](https://developer.android.com/studio/)

Android SDK used to provide all the necessary developer tools to build, test, and debug apps for Android in Windows, Mac or Linux.

4. [Android Build Tools](https://developer.android.com/studio/releases/build-tools)

Android SDK build tools used to debug, build, run and test an Android application.


## How to contribute

All contributions are welcome, from code to documentation to graphics to design suggestions to bug reports. Please use GitHub to its fullest. Whatever you have to offer, we can use it!


## Support & Contact

- Mobile number: (+254) 798731203

- Email Address: collo.kariss@gmail.com

- github-username: [zecollokaris](https://github.com/zecollokaris)

## LICENSE

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.