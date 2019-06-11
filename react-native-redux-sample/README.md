# Sample JavaScript React-Native Redux

SendBird React-Native sample using [SendBird SDK](https://github.com/sendbird/SendBird-SDK-JavaScript).

## Prerequisite

- [Node](https://nodejs.org/en/)
- [NPM](https://www.npmjs.com/)
- [Cocoapods](https://cocoapods.org/)
- [XCode](https://developer.apple.com/xcode)
- [XCode Command Line Tools](https://facebook.github.io/react-native/docs/getting-started.html#xcode)
- [Android Studio](https://developer.android.com/studio/) (+Android SDK/Google API)

## Run the sample

1. Install React Native CLI.

        npm install -g react-native-cli

2. Install required packages.

        npm install

3. (iOS only) Pod install.

        cd ios
        pod install

4. (iOS only) Add library in XCode

- Open XCode and load workspace
- Right click to 'Libraries' > Add Files to "Project Name" > select `node_modules/react-native/Libraries/PushNotificationIOS/RCTPushNotification.xcodeproj`
- Right click to 'Libraries' > Add Files to "Project Name" > select `node_modules/react-native-gesture-handler/ios/RNGestureHandler.xcodeproj`
- Project Settings > Build Phases > Link Binary With Libraries > Add `libRCTPushNotification.a`
- Project Settings > Build Phases > Link Binary With Libraries > Add `libRNGestureHandler.a`
- Project Settings > Build Phases > Link Binary With Libraries > Add `JavaScriptCore.framework`

5. Run the sample. Before starting, you should launch device amulator (or actual device) to run the sample in Android. This sample is not available for real device in iOS due to Apple Development Policy. In order to run React Native sample in real device, follow [React Native official guide](https://facebook.github.io/react-native/docs/running-on-device.html) for your own setup.

        react-native run-android
        react-native run-ios