# features

## getting started

1. dependency graph built by webpack. Use import/export commands of ES2015 to make it
1. npx webpack is the basic command to execute webpack and create its dist folder

## assets management

### css loader

1. style-loader and css-loader used to load css files
1. style-loader injects inline styles into DOM
1. css-loader take the css styles defined in files and create an injectable inline style to insert in \<head>\</head>

### images loader

1. we have to check difference between file-loader and "type: 'asset/resource'". At the moment we used the second one and not the file loader
