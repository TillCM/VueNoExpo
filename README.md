# VueNative app without Expo :

### Setup Environment
1. Follow instructions from here to install Android Studio and setup the environment: [Set up Android Environment](https://reactnative.dev/docs/environment-setup)
2. Setup the React Native Environment without Android Studio: [Setup Environment Without Android Studio](https://medium.com/@rodrigoklosowski/an-updated-guide-to-installing-react-native-without-android-studio-e3a87b4e1112)

### Install GenyMotion emulator and set up for Visual Studio Code
1. Follow instructions from here: [Install GenyMotion](https://codeloop.org/connect-genymotion-emulator-with-react-native/)

### NNB make sure that you set the following environment variables:

ADNROID_HOME (Pointing to where your Android SDK is installed )
ANDROID_SDK_ROOT (Pointing to where your Android SDK is installed )
 (user and system for Windows)
 Seta PATH variable for your platform tools (Pointing to the platofrom tools inside the Andoid SDK Folder)

```ANDROID_HOME               %LOCALAPPDATA%\Android\Sdk```

```ANDROID_SDK_ROOT           %LOCALAPPDATA%\Android\Sdk```

```Path to tools %LOCALAPPDATA%\Android\Sdk\platform-tools```

## Linux Environment Setup:

1. Download 

## Start the GenyMotion Emulator and run your app with :

```react-native run-android```

### Create Hello World  app.:

1. Install the vue native cli : ```npm install --global vue-native-cli```

2. Install the react-native cli: ```npm install --global react-native-cli```

3. Create your application: ```vue-native init <projectName> --no-expo```

4. Edit the following in the android/app/build.gradle file by adding

```bundleInDebug:true```

```
project.ext.react = [
    bundleInDebug: true,
    enableHermes: false,  // clean and rebuild if changing
]
```

5. Run your application with:

```react-native run-android```

OR

```react-native run-ios --simulator "iPhone 8"```




