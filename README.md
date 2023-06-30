## Background

This zero dependency package provides a metro config to enable web5 to work on react native

## Usage

Install package:

```js
yarn add @tbd54566975/web5-react-native-metro-config
```

Add the package to your metro config.

Expo:

```js
// Learn more https://docs.expo.io/guides/customizing-metro
const { getDefaultConfig } = require('expo/metro-config');
const { mergeConfig } = require('metro-config');

const config = getDefaultConfig(__dirname);
const web5Config = require('@tbd54566975/web5-react-native-metro-config');

module.exports = mergeConfig(config, web5Config);
```

React Native:

```js
const { getDefaultConfig, mergeConfig } = require('metro-config');

const config = getDefaultConfig(__dirname);
const web5Config = require('@tbd54566975/web5-react-native-metro-config');

module.exports = mergeConfig(config, web5Config);
```
