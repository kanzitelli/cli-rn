<img src="https://i.postimg.cc/3J7cRXTs/cli-rn-gif.gif" width="100%" title="Logo">

Purpose of [cli-rn](https://github.com/kanzitelli/cli-rn) is to simplify and accelerate the process of React Native App development. It is not a replacer for react-native cli but a good addition!

### Quick start

```bash
> npm i -g cli-rn
> cli-rn new AppName
```

It will generate a new production-ready React Native App bootstrapped from [rn-starter](https://github.com/kanzitelli/rn-starter) with [React Navigation](https://github.com/react-navigation/react-navigation) preconfigured.

If you'd like to use [React Native Navigation](https://github.com/wix/react-native-navigation) by Wix, you can run:

```bash
> cli-rn new AppName -n rnn
```

Example with all possible options:

```bash
> cli-rn new MyNewApp -b com.mycompany.MyNewApp -n rn
```

#### > cli-rn --help

```
Usage: cli-rn [options] [command]

Options:
  -h, --help               display help for command

Commands:
  new [options] <appName>  generates a new production ready React Native App
  help [command]           display help for command
```

#### > cli-rn new --help

```
Usage: cli-rn new [options] <appName>

generates a new production ready React Native App

Options:
  -n, --navigation <navigation>  navigation option. Possible values: ['rn', 'rnn'].
                                 Default: 'rn'.
  -b, --bundleId <bundleId>      bundle identifier. Default: 'clirn.app.<appName>'
  -h, --help                     display help for command
```

### Starters

- [rn-starter](https://github.com/kanzitelli/rn-starter) - 🦄 Production-ready starter for your next React Native App! Powered by cli-rn, React Navigation (v6), RN UI lib, Mobx, Reanimated 2, Dark Mode, Localization, Notifications, Permissions, and much more.
- [rnn-starter](https://github.com/kanzitelli/rnn-starter) - 🤹 Production-ready starter for your next React Native App! Powered by cli-rn, React Native Navigation, RN UI lib, Mobx, Reanimated 2, Dark Mode, Localization, Notifications, Permissions, and much more.

### Worth checking

#### Articles

- cli-rn — making RN app developing experience as smooth as possible - [Medium](https://kanzitelli.medium.com/cli-rn-making-rn-app-developing-experience-as-smooth-as-possible-1022aae3a0d3), [Dev.to](https://dev.to/kanzitelli/cli-rn-making-rn-app-developing-experience-as-smooth-as-possible-4e98)
