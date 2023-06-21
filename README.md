# react-native-theme-control

Control the native platform theme from React Native.

✅ Control theme of RN Views, as well as native UI controls (alerts, native menus, date pickers... on both Android and iOS)

✅ Recover the theme upon app startup

✅ Supports Expo via a config plugin

✅ New architecture supported

Additionally, provides functionality to control the appearance (background and border color, light / dark buttons) of the Android navbar.

The package is tested with RN >= 0.66.1 (last tested with RN 71, Expo 48).

## Motivation

The use case for the package is explained in a [youtube video](https://youtu.be/NNYQj_T0Sf8).

In React Native, you can use the `useColorScheme()` hook, or other functions from the `Appearance` API to get information about the system theme.

Using that information, you can then render your Views in dark or light mode design. However, that information is read-only: you cannot influence what the `useColorScheme()` hook returns. What if you want to allow the user to choose the application theme? React Native core does not directly expose the APIs to do so.

You might follow one of the many blog posts for theming React Native apps such as [here](https://blog.logrocket.com/comprehensive-guide-dark-mode-react-native/#dark-mode-react-native-using-context-api) or [here](https://medium.com/@ratebseirawan/react-native-dark-mode-done-right-13f83b39a4ca). The approach taken by the guides is to store the application theme in the JavaScript part of your app. However, this can easily leave your users with a broken experience because while the React Native views will be rendered correctly, the native views (Alert, Document picker, Date picker, Menu...) will not.

This package provides a solution to change the application theme so that both react native and native components use the same theme - see the [relevant part of the video](https://youtu.be/NNYQj_T0Sf8?t=73).


## This Package Was Sponsorware 💰💰💰

This package was only available to my GitHub Sponsors: TODO tweet

Enjoy, and thanks for the support! ❤️

Sponsorware idea is not mine, learn more about **Sponsorware** at [github.com/sponsorware/docs](https://github.com/sponsorware/docs) 💰.

I simply adopted it because making open source is a lot of fun but is not sustainable without compensation.

## Documentation

Installation and usage instructions can be found [here](./docs/install.md).

The library api is documented in detail [here](./docs/readme-internal.md).

More usage examples can be found [in the example project](./example).

### Credits

Some naming inspiration for the Android Navbar components was taken from [react-native-bars](https://github.com/zoontek/react-native-bars).

## License

MPL-2.0
