# SETUP

A simple development setup for Linux using Expo Managed Workflow (Expo GO).

## Requirements

- NodeJS
- Expo CLI (local)
- Expo GO ([Android](https://play.google.com/store/apps/details?id=host.exp.exponent) app)

## Getting Started

```bash
# To always get the latest version, do not install expo-cli globally
# Use npx instead
$ npx expo --version

# removing the global version, if `expo --version` return a version
$ npm uninstall -g expo-cli

# To create a new project
$ npx create-expo-app

# Working with the web version
$ npm run web

# Working with the Android version
$ npm run start
# Then, open the Expo app and scan the QR Code
```