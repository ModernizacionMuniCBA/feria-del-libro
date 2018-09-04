## De HTML5 a APK vía Cordova

Actualizacion 2018 del compilador de la app

Da error al compilar
```
cordova build android
```

```
cordova platform update android
```
Dice:
```
Using cordova-fetch for cordova-android@~7.0.0
Updating android project...
(node:26900) UnhandledPromiseRejectionWarning: An in-place platform update is not supported. 
The `platforms` folder is always treated as a build artifact in the CLI workflow.
To update your platform, you have to remove, then add your android platform again.
Make sure you save your plugins beforehand using `cordova plugin save`, and save 
a copy of the platform first if you had manual changes in it.
	cordova plugin save
	cordova platform rm android
	cordova platform add android

```

Ahora la compilacion (básica) funciona OK.

