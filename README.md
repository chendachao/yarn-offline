
https://yarnpkg.com/blog/2016/11/24/offline-mirror/



`yarn config set yarn-offline-mirror ./npm-packges-offline-cache`


`yarn config set yarn-offline-mirror-prune true`


Cut from home directory's .yarnrc file to this project's .yarnrc

```
yarn-offline-mirror "./npm-packges-offline-cache"
yarn-offline-mirror-prune true
```

`rm -rf node_modules/ yarn.lock`
`yarn install`

## Test

`yarn cache clean`

disconnect the network

`yarn install --offline`

