# Hermanoemos

## To run:
```
npm start
get the expo app on phone
on browser, select tunel near the qr code and wait
scan the new qr code
```

## To optmize and build
First you will need to have sure of some things. First is in app.json have a "package" under android with your package name For last make sure you have installed `npm install sharp-cli`  
```
npx expo-optimize
expo build:android -t apk
```

## To build without expo
```
expo eject
npm install
cd android && ./gradlew assembleRelease
```
When finished the app will be in `android/app/build/outputs/apk/release/`
After this discard all the changes and delete folder android and ios.

In case of error, discard everything, restart the PC and run again the commands.
