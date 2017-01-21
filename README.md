# Weatherbee 100 Wrapper

This is a [Cordova-based](https://cordova.apache.org/) wrapper application for the [Weatherbee 100 Ventilator Simulation App](https://github.com/nickcherry/weatherbee_100).

## Development Setup

### Installing Dependencies

After installing [Node](https://nodejs.org/en/) and [NPM](https://www.npmjs.com/), run the following command to install Cordova globally:

```shell
npm install -g cordova
```

After dependencies have been installed, run the iOS app locally by running the following command from the project root:

```shell
cordova run ios
```

## Updating Assets

To update the assets (i.e. the actual application), pull down the [weatherbee_100](https://github.com/nickcherry/weatherbee_100) repository, install dependencies, and run the following from _that_ project's root:

```shell
npm run build
```

This will generate a `build` directory (in the __weatherbee_100__ project), whose contents should then be copied over to the __weatherbee_100_wrapper__ project's `www` directory. Rebuild the wrapper application by running the following:

```shell
cordova build
```
