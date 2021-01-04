# ouput management

## preparation

1. in webpack.config.js u can set more than one entry points by splitting them out.
1. in output object u can use filename: '[name].bundle.js' to create one file for each entry in entry object above.

## html-webpack-plugin

1. by default it will generate its own index.html in dist folder so if u have already one it will be replaced.
1. it has to be added in plugins array in webpack.config.js and can take into the various parameters
