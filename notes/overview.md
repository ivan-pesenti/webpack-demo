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

### fonts loader

1. download font-family in assets folder.
1. use type: 'asset/resource'
1. inject in css stylesheet through the @font-face syntax

### data loader

1. to import json no changes needed
1. changes needed to import xml, csv, tsv
1. pay attention to curly braces as u haven't to use them to import data. if u are unsure no put them at all!
