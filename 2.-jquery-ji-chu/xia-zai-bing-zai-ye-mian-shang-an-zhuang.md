# 2.1 安裝 jQuery

## 方式一：自行下載安裝

點進去[官網網址](https://jquery.com/)後，如下圖，看到「Download jQuery」按鈕，點進去。

<figure><img src="../.gitbook/assets/jquery_download (2).png" alt=""><figcaption></figcaption></figure>



在 **`jquery/practice/vendors/jquery/`** 資料夾中，建立檔名 **`jquery-4.0.0.min.js`** ，然後將原始碼全部複製，貼進剛建立的檔案並儲存。

然後在頁面上載入，開啟 `jquery/practice/index2.html` 檔案，改成如下(載入 jQuery 檔案，放在 **`</body>`** 之前)：

```html
<!doctype html>
<html lang="zh-Hant">
  <head>
    <meta charset="utf-8">
    <title>jQuery 相關練習</title>
  </head>
  <body>
    
    <script src="./vendors/jquery/jquery-4.0.0.min.js"></script>
  </body>
</html>
```

在該頁面就可以使用 jQuery 函式庫了。



## 方式二：在 CodePen 上安裝

例：[https://codepen.io/editor/carlos411/pen/01a1d864-66bf-7119-b826-b119ecbe47e9](https://codepen.io/editor/carlos411/pen/01a1d864-66bf-7119-b826-b119ecbe47e9)

{% embed url="https://codepen.io/editor/carlos411/pen/01a1d864-66bf-7119-b826-b119ecbe47e9" %}

