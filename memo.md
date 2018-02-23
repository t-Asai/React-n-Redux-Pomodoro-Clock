$ yarn run
でbundleを選ぶと、
```
NODE_ENV=production ./node_modules/.bin/webpack -p --config webpack.config.js
```
とあるように
> webpack.confing.js
を読みに行ってくれる模様

webpack.confing.js
を見ると
entryで
> './app/core.js'
とあるので、core.jsを読みに行ってくれている
bundleした結果はbundle.js

core.jsでは自作コードの諸々をimportしてる

ただ、これはreactのコードであってnativeのコードではなかったから
iosのbuildとかがなかったのか
理解