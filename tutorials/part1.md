## 專案環境設立

### 設定 CSS Module
此做法主要是能夠對 CSS 模組產生優化，方便使用 CSS 檔案。

```bash
yarn eject
```


開啟 `webpack.config.dev` 找到 `css` 修改裡面參數，使得可以直接使用 css module

<img src-"/tutorials/Images/img1070212-1.png">
<img src-"/tutorials/Images/img1070212-2.png">


```js
 options: {
    importLoaders: 1,
    modules:true,
    localIdentName: '[name]__[local]__[hash:base64:5]'
  }
```

## 加入字體
使用 [Google Font](https://fonts.google.com/?selection.family=Open+Sans:400,700)，並使用 CDN 匯入再 insex.html
