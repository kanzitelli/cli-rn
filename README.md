<img src="https://i.postimg.cc/3J7cRXTs/cli-rn-gif.gif" width="100%" title="Logo">

> Currently in very `alpha` stage and under heavy testing. Available for iOS only.

Purpose of [cli-rn](https://github.com/kanzitelli/cli-rn) is to simplify and accelerate the process of app development.

*cli-rn* will help you to generate a production-ready app and test it remotely using **[cli-rn app](https://github.com/kanzitelli/cli-rn-app)**.

### Quick start
```bash
> npm i -g cli-rn
> cli-rn new AppName
```
It generates a new production-ready app bootstrapped from [rnn-starter](https://github.com/kanzitelli/rnn-starter).

### Testing
In order to start testing an app you develop on your local machine, you will need a real device to install **[cli-rn app](https://github.com/kanzitelli/cli-rn-app)** in Release mode. Follow the steps on **[cli-rn app](https://github.com/kanzitelli/cli-rn-app)** page.

Once you install the **cli-rn app**, you should `cd` to the root of an app you develop.

> There are two modes: `DEV` and `PROD`.
When testing in `DEV` mode, you need to have Metro bundler running (`yarn start`) as **cli-rn** relies on it when exposing tunnel.
When testing in `PROD` mode, **cli-rn** generates an app bundle and exposes tunnel to that file.
For more "Things to be aware of", please check the **[following section](https://github.com/kanzitelli/cli-rn-app#things-to-be-aware-of)**.

```
> cd AppName
> cli-rn remote:dev # DEV mode
> cli-rn remote:prod # PROD mode
```
The steps above can take some time when doing it for the first time.

After it's done, you should see something like on the image below
<img src="https://i.postimg.cc/m2gpGbRM/Screenshot-2021-01-11-at-20-39-29.png" width="100%" title="AppCodeCLI">
The generated `App Code` has to be put in **cli-rn app** as shown [here](https://github.com/kanzitelli/cli-rn-app#app-interface).

Happy testing! 🤙

### > cli-rn help
```
Usage: cli-rn [options] [command]

Options:
  -h, --help               display help for command

Commands:
  new [options] <appName>  generates a new production-ready app bootstrapped from kanzitelli/rnn-starter
  remote:dev               opens tunnel to 8081 port where Metro bundler should be running so you are able to test the app through cli-rn app
  remote:prod              opens tunnel to release bundle
  app                      generates cli-rn app on your local machine
  app:info                 information about cli-rn app
  help [command]           display help for command
```

### Motivation
You may come up with the questions like `Why?` and `What for?` if there is [Expo](https://expo.io) which does all of those steps much better. I would say that this is just `out-of-curiosity` and yes, I love to automate the routine!

I have been developing the app ([Christmas Market](https://apps.apple.com/ru/app/id1446775875)) recently with [react-native-navigation](https://github.com/wix/react-native-navigation) and it contains some cool animations. As animations (anyways) lag in dev mode, I had to launch the app in release mode a few times in an hour to test animations' smoothness. And I got bored of waiting and decided to start a research on how I can automate this process. Plus, we can see that it is possible and done by Expo.

- 💚 Thanks to [React Native](https://reactnative.dev).
- 💙 Thanks to [Expo](https://expo.io) for insipration
- ❤️ Thanks to [Wix team](https://github.com/wix) for initiating [react-native-navigation](https://github.com/wix/react-native-navigation) and all contributors for maintaining it
