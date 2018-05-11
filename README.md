
# react-native-star-prnt

## Getting started

`$ npm install react-native-star-prnt --save`

### Mostly automatic installation

`$ react-native link react-native-star-prnt`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-star-prnt` and add `RNStarPrnt.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNStarPrnt.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Add $(PROJECT_DIR)/../node_modules/react-native-star-prnt/ios/Frameworks to Framework search paths

for Bluetooth printers:

1. Click on the information property list file (default : “Info.plist”).
2. Add the “Supported external accessory protocols” Key.
3. Click the triangle of this key and set the value for the “Item 0” to “jp.star-m.starpro”.


#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNStarPrntPackage;` to the imports at the top of the file
  - Add `new RNStarPrntPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-star-prnt'
  	project(':react-native-star-prnt').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-star-prnt/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-star-prnt')
  	```

#### Windows
[Read it! :D](https://github.com/ReactWindows/react-native)

1. In Visual Studio add the `RNStarPrnt.sln` in `node_modules/react-native-star-prnt/windows/RNStarPrnt.sln` folder to their solution, reference from their app.
2. Open up your `MainPage.cs` app
  - Add `using Star.Prnt.RNStarPrnt;` to the usings at the top of the file
  - Add `new RNStarPrntPackage()` to the `List<IReactPackage>` returned by the `Packages` method


## Usage
```javascript
import RNStarPrnt from 'react-native-star-prnt';

// TODO: What to do with the module?
RNStarPrnt;
```
  