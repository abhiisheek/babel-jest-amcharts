# babel-jest-amcharts

[Babel](https://github.com/babel/babel) [jest](https://github.com/facebook/jest) plugin to be used with [amCharts](https://www.amcharts.com/)

## Usage

If you are already using `jest-cli`, just add `babel-jest-amcharts` and it will automatically compile JavaScript code using Babel.

```bash
npm install --D babel-jest-amcharts @babel/core
```

## Setup

_Note: this step is only required if you are using `babel-jest` with additional code preprocessors._

To explicitly define `babel-jest-amcharts"` as a transformer for your JavaScript code, map _.js_ files to the `babel-jest` module.

```json
"transform": {
  "^.+\\.(js|jsx)$": "babel-jest-amcharts"
},
```

And exclude _@amcharts_ files from being skipped for tarnsformation by `jest`.

```json
"transformIgnorePatterns": [
  "[/\\\\]node_modules[/\\\\](?!(@amcharts)\\/).+\\.(js|jsx|ts|tsx)$"
],
```
