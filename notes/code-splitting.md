## overview

1. it allows to split your code among different bundles
1. they can be loaded in parallel or in demand
1. speed up the load time if used correctly

## entry points

1. manually split your file in entry object in webpack.config.js
1. cons:
   - duplicated modules will be included in both bundles
   - not flexible and cannot dynamically split code

### prevent duplication

### entry dependencies

1. use the dependOn option
1. change the entry object in webpack.config.js
1. if u use multiple entry points in a single HTML page, sets the optimization.runtimeChunk to 'single'

#### SplitChunksPlugin

1. change the optimization object in webpack.config.js

## dynamic import

1. remove static import at the top of the file (in js file)
1. dynamically import modules in code
1. the import() syntax returns a promise so it can be used also in async version

## prefetch/preload modules

1. prefetch: resource may be needed for future navigation
1. preload: resource needed also for the current navigation
1. example of prefetch is when the login opens up a modal. this modal has be shown on click of login btn. in idle time this can be prefetch by webpack
1. preload starts to load in parallel as its parent and not only when the parent is loaded
