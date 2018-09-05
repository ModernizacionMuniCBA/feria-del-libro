## De HTML5 a APK vía Cordova

Actualizacion 2018 del compilador de la app

Da error al compilar la del año pasado por versiones de pluguins y cordova.

Variables de entorno

export ANDROID_HOME=/home/USER/Android/Sdk
export PATH=${PATH}:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools

Solo la primera vez:
```
cordova create feria ar.gob.cordoba.gobiernoabierto.feriadellibro FeriaDelLibro
cordova platform add android
```

Todas las compilaciones:
```
cordova build
```

### Firmar la app

Instrucciones [acá](https://developer.android.com/studio/publish/app-signing).  

```
cordova build android --release

jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore agenda-de-la-feria-key.keystore platforms/android/app/build/outputs/apk/release/app-release-unsigned.apk AgendaDeLaFeria

# si ya existe
rm platforms/android/app/build/outputs/apk/release/AgendaDeLaFeria-release.apk

zipalign -v 4 platforms/android/app/build/outputs/apk/release/app-release-unsigned.apk platforms/android/app/build/outputs/apk/release/AgendaDeLaFeria-release.apk
```





