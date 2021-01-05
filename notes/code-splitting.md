## overview

1. it allows to split your code among different bundles
1. they can be loaded in parallel or in demand
1. speed up the load time if used correctly

## three modes

### entry points

1. manually split your file in entry object in webpack.config.js
1. cons:
   - duplicated modules will be included in both bundles
   - not flexible and cannot dynamically split code
