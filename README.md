# Template React Native app
> React Native project

## Setup
Checkout the project  

Install dependencies
```
yarn install

```
To rename the project to your app name
```
yarn global add react-native-rename

react-native-rename <newName>
```
For iOS, you must do a pod install
```
cd ios && pod install && cd ..
```

Run the project
```
react-native run-ios
```
or
```
react-native run-android
```

### Troubleshooting
There seems to be an issue with the debug keystore generation when running react-native run-android, if you get the error "Keystore file '/Project-Folder/android/app/debug.keystore' not found for signing config 'debug'"
download [the original keystore](https://raw.githubusercontent.com/facebook/react-native/master/template/android/app/debug.keystore) 
file from the official template and out it in `android/app`.  
See [this issue](https://github.com/facebook/react-native/issues/25629) for more information.
