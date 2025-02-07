# Expo CLI Build Failure: Custom Babel Configuration Conflict

This repository demonstrates a bug where using a custom Babel configuration with Expo CLI leads to build failures.  The error arises from a conflict between Expo's default Babel setup and the custom configuration, often due to plugin or preset incompatibilities.

## Reproducing the bug

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Attempt to run `expo start` or `expo build:ios/android`. 

The build process will likely fail with unhelpful error messages related to Babel.

## Solution

The solution involves carefully integrating the custom Babel configuration with Expo's configuration, ensuring no conflicts arise between plugins or presets. The corrected `babel.config.js` file in the `solution` branch demonstrates one approach to resolving this conflict.
