
# LAPO-Mobile-Wallet-Core

## Getting started

Add to your package.json like 

```$xslt
dependencies: {
    ...
    "lapo-core": "git+ssh://git@github.com/LapoLab/LAPO-Mobile-Wallet-Core.git",
    ...
}
```

and install via `npm i` or `yarn`

### Mostly automatic installation

`$ react-native link lapo-core`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `lapo-core` and add `RNLapoCore.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNLapoCore.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNLapoCorePackage;` to the imports at the top of the file
  - Add `new RNLapoCorePackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':lapo-core'
  	project(':lapo-core').projectDir = new File(rootProject.projectDir, 	'../node_modules/lapo-core/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':lapo-core')
  	```


## Usage
```javascript
import RNLapoCore from 'lapo-core';

// TODO: What to do with the module?
RNLapoCore;
```
