# Expo Android Build Failure: react-native-reanimated Linking Errors

This repository demonstrates a bug encountered when building an Android app using Expo CLI and the `react-native-reanimated` library. The build process fails due to issues with native module linking, resulting in errors related to undefined symbols. This issue manifests even if the JavaScript code using `react-native-reanimated` appears to be correct.

## Bug Description

The problem arises during the Android build process when Expo attempts to link the native modules required by `react-native-reanimated`.  This results in build failures with error messages indicating that certain symbols cannot be found. 

## Reproduction Steps

1. Clone this repository.
2. Run `npm install` or `yarn install` to install dependencies.
3. Attempt to build the Android app using Expo CLI (e.g., `expo build:android`).

## Solution

The provided solution demonstrates how to fix this problem by ensuring correct linking and configuration of the `react-native-reanimated` library during the Expo build process.  A common solution involves explicitly configuring native modules and ensuring all necessary dependencies are correctly installed and linked.  Sometimes cleaning the build cache and reinstalling packages can resolve issues.