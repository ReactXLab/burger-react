

```bash
yarn eject
```


開啟 `webpack.config.dev` 找到 `css` 修改裡面參數，使得可以直接使用 css module



```js
 options: {
    importLoaders: 1,
    modules:true,
    localIdentName: '[name]__[local]__[hash:base64:5]'
  }
```
