<img src="https://i.postimg.cc/3J7cRXTs/cli-rn-gif.gif" width="100%" title="Logo">

Purpose of [cli-rn](https://github.com/kanzitelli/cli-rn) is to simplify and accelerate the process of React Native App development. It is not a replacer for react-native cli but a good addition!

## Quick start

```bash
> npx cli-rn new App

# or install it globally first
> npm i -g cli-rn
> cli-rn new App
```

It will generate a new production-ready Expo (React Native) App bootstrapped from [expo-starter](https://github.com/kanzitelli/expo-starter).

For [React Native Navigation](https://github.com/wix/react-native-navigation) (by Wix) setup:

```bash
> cli-rn new App -t rnn
```

For [React Navigation](https://github.com/wix/react-native-navigation) (w/out Expo) setup:

```bash
> cli-rn new App -t rn
```

Example with all possible options:

```bash
> cli-rn new App -b com.company.App -t expo
```

### > cli-rn new --help

```
Usage: cli-rn new [options] <App>

Generates a new production ready React Native App. Try it: > cli-rn new app

Options:
  -t, --template <template>  Template option. Possible values: ['expo', 'rn', 'rnn']. Default: 'expo'.
  -b, --bundleId <bundleId>  Bundle identifier. Default: 'clirn.<app>'. This option will be ignored for 'expo' template.
  -h, --help                 display help for command
```

### Starters

- [expo-starter](https://github.com/kanzitelli/expo-starter) - 🦥 Production-ready starter for Expo (React Native) App! Powered by cli-rn, React Navigation (v6), RN UI lib, Mobx, Reanimated 2, Dark Mode, Localization, and much more.
- [rn-starter](https://github.com/kanzitelli/rn-starter) - 🦄 Production-ready starter for your next React Native App! Powered by cli-rn, React Navigation (v6), RN UI lib, Mobx, Reanimated 2, Dark Mode, Localization, Notifications, Permissions, and much more.
- [rnn-starter](https://github.com/kanzitelli/rnn-starter) - 🤹 Production-ready starter for your next React Native App! Powered by cli-rn, React Native Navigation, RN UI lib, Mobx, Reanimated 2, Dark Mode, Localization, Notifications, Permissions, and much more.

### Worth checking

#### Articles

- cli-rn — making RN app developing experience as smooth as possible - [Medium](https://kanzitelli.medium.com/cli-rn-making-rn-app-developing-experience-as-smooth-as-possible-1022aae3a0d3), [Dev.to](https://dev.to/kanzitelli/cli-rn-making-rn-app-developing-experience-as-smooth-as-possible-4e98)
