
# nwapplogger-react-native-sdk

## Getting started

`$ npm install nwapplogger-react-native-sdk --save`

### Mostly automatic installation

`$ react-native link nwapplogger-react-native-sdk`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `nwapplogger-react-native-sdk` and add `RNReactNativeNwAppLogger.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNReactNativeNwAppLogger.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNReactNativeNwAppLoggerPackage;` to the imports at the top of the file
  - Add `new RNReactNativeNwAppLoggerPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':nwapplogger-react-native-sdk'
  	project(':nwapplogger-react-native-sdk').projectDir = new File(rootProject.projectDir, 	'../node_modules/nwapplogger-react-native-sdk/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':nwapplogger-react-native-sdk')
  	```

## Usage
```javascript
import NWAppLogger from 'nwapplogger-react-native-sdk';

// TODO: What to do with the module?
NWAppLogger;
```
  