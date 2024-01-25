## Install it!

```shell
npm i @fjrodafo/colors
```

## Run it!

```mjs
// Import the module
import cf from "@fjrodafo/colors"
```

```mjs
// It will display a formatted color message
console.log(
    cf.italic(`I see a ${cf.bgRed("red")} car and I ${cf.bold("want")} it painted ${cf.black("black")}.`)
)
```

## Usage

This library provides an object which includes a variety of text coloring and formatting functions.

The object includes following coloring functions: `black`, `red`, `green`, `yellow`, `blue`, `magenta`, `cyan`, `white`, `gray`.

The object also includes following background color modifier functions: `bgBlack`, `bgRed`, `bgGreen`, `bgYellow`, `bgBlue`, `bgMagenta`, `bgCyan`, `bgWhite`.

Besides colors, the object includes following formatting functions: `dim`, `bold`, `hidden`, `italic`, `underline`, `strikethrough`, `reset`, `inverse`.

## Additional utilities

The library provides additional utilities to ensure the best results for the task:

- `isColorSupported` - boolean, explicitly tells whether or not the colors or formatting appear on the screen.

    ```mjs
    if (cf.isColorSupported) {
        console.log("Yay! This script can use colors and formatters")
    }
    ```

- `createColors(enabled)` - a function that returns a new API object with manually defined color support configuration.

    ```mjs
    let { red, bgWhite } = cf.createColors(options.enableColors)
    ```

## Links

Full repository on [github](https://github.com/FJrodafo/npm-colors)/[gitlab](https://gitlab.com/FJrodafo/npm-colors).

Visit the npm package website [here](https://www.npmjs.com/package/@fjrodafo/colors).