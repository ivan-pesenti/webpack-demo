# development

tool in this guide have to be used only for development purposes.
do not use them in production!!!

## source maps

1. if u bundle all your source files into one it can be difficult to track down where errors or warning come from.
1. let's suppose that u have a.js, b.js and c.js and one raises an error. u have only bundle.js which wrap all of the three. with source maps u can know which file broke.
1. map compiled code to the original source code

## choosing a development tool

### using watch mode

1. u have to add a scripts in package.json in scripts section.
1. run it with "npm run watch"
1. the process listens to changes in dependency graph and it recompiles the changed modules without have to rebuild it manually
1. change the options of clean-webpack-plugin
1. main downside it that u have to manually refresh the browser in order to see the changes

### webpack-dev-server

1. has to be configured within devServer object in webpack.config.js to set the directory where to look for the files.
1. default url localhost:8080
1. u've to had a scripts in package.json "start": "webpack serve --open"
1. it opens up the browser and u don't have to manually refresh to see changes in action

### webpack-dev-middleware

1. it emits file to a server.
1. it's used internally also by webpack-dev-server but u can install it as a separate package to obtain a more customizable setup.
1. it's run together with 'express'
1. u've to manually setup a server using npm package 'express'
1. have to add an entry in scripts in package.json to run the node server setup in server.js => "server": "node server.js"
1. drawback: have to manually refresh the browser to see changes
