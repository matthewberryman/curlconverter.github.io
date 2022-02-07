A static Web app for showing off [curlconverter](https://github.com/curlconverter/curlconverter)

Uses Webpack

curlconverter uses [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for Bash parsing, which adds some complexity to deployment because we have to copy the generated WASM files from `node_modules/` to serve them. See [webpack.config.js](webpack.config.js) for details.

# pre-setup
    npm install -g serve
# setup

    npm install
    npm run build
    serve dist
