# Basic Webpack 5 Setup with SASS, Babel, PostCSS, Self-hosted fonts and SVG Sprite

**Important**: It is assumed that you have `node.js` installed on your computer.

## webpack.config.js and package.json

### webpack.config.js

Note that by default, the path to the production folder is set as `dist` by default:

- `path: path.resolve(__dirname, "dist"),`.

However, I've changed the output folder to `docs` (which makes publishing to Git Pages much simpler):

- `path: path.resolve(__dirname, "docs"),`.

Also,   

`
  devServer: {
    static: ["./dist"],
  },
  
  
has been changed to:

`
  devServer: {
    static: ["./docs"],
  },
`
### package.json

Similarly, all references in this file to `./dist` have been changed to `./docs`.

## Description

This repository can be used to build a simple one-page website (i.e not React or equivalent). If you use it you can be sure that:

- Modern Javascript will work on older browsers,
- `.scss` files compile to CSS (usingthe new Dart SASS implementation which allows files to be imported with `@use` and `@forward`, replacing the now deprecated `@import`), and
- the compiled CSS will work on older browsers,
- You will also be able to easily publish the page to Git Pages.

For more information see my [One Page Site Template](https://github.com/chrisnajman/one-page-site-template/tree/main) (GitHub).


## Credits

- I got most of the setup done by following the tutorials by **Swashbuckling with Code**, especially [Creating and Understanding a Basic Webpack 5 Setup](https://www.youtube.com/watch?v=X1nxTjVDYdQ&list=PLmZPx_9ZF_sB4orswXdpThGMX9ii2uP7Z&index=1).

## Useful Links

- [PNG to WEBP conversion](https://onlineconvertfree.com/complete/png-webp/)
- [Favicon converter](https://favicon.io/favicon-converter/)
- [Boxicons (SVGs)](https://boxicons.com/)
- [SVG Editor](https://svgeditoronline.com/editor/)
- [Font size clamp generator](https://clamp.font-size.app/)


## Git Pages

[Website (Git Pages)](https://chrisnajman.github.io/webpack5-basic-setup)
