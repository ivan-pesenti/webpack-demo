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
