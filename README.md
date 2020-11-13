# expo-ota
Ejected managed workflow to bareflow using 'expo eject'.
Expo-updates configurations will be done automatically in both android and ios folder.
After that, apk was built in react-native cli and app was installed. Then changes were made in the project and published using 'expo publish' which successfully created and published app bundles to expo account and a URL was provided in order to compare and check for updates. Changes were visible in the app after reload.

### Commands for Managed workflow
expo init //initializes project \
yarn add expo-updates //adding package for updates \
expo build:android //for android build and similar for ios \
expo publish //provides with expo URL to check for updates

### Commands for Bare workflow
expo eject \
//configurations of expo-updates will be done automatically \
//built apk for android \
react-native run-android --variant=release

### Ways to host updates
Updates and their respective assets (JavaScript bundles, images, fonts, etc.) can be hosted on a server somewhere that deployed client apps can access. expo-cli provides a couple of easy options for this: \
(1) expo export creates prebuilt update packages that you can upload to any static hosting site (e.g. GitHub Pages), and \
(2) expo publish packages and deploys your updates to Expo's updates service, which is part of the Developer Services we offer.\
You can also run your own server to host your updates, provided it conforms to the protocol expo-updates expects. You can read more about requirements in the link provided.

### References
https://docs.expo.io/bare/updating-your-app/ <br/>
https://docs.expo.io/versions/latest/sdk/updates/ <br/>
https://docs.expo.io/guides/configuring-ota-updates/ \
https://docs.expo.io/distribution/hosting-your-app/


