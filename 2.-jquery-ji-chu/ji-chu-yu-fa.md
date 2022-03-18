# 2.2 試試看：基本語法

## jQuery 及 $

使用 jQuery 的前綴詞，可使用以下兩個方式：

```javascript
jQuery
```

等同於：

```javascript
$
```



執行：

```
console.log(jQuery);
console.log($);
```

結果如下圖：

![](../.gitbook/assets/jquery\_func.png)

是一樣的東西，其實 jQuery 只是一個函式。



## 試試看：jQuery 基本語法

以下請編輯 `jquery/practice/index_test.html` 檔案，將使用 jQuery 語法的程式，放在以下位置：

```markup
<!doctype html>
<html lang="zh-Hant">
  <head>
    <meta charset="utf-8">
    <title>jQuery 相關練習</title>
  </head>
  <body>
    
    <p class="test">這是段落</p>
    
    <script src="./vendors/jquery/jquery-3.4.1.min.js"></script>
    <script>
      // 相關 jQuery 語法，寫在這裡，也就是要在 jquery 函式庫載入之後。
    </script>
  </body>
</html>
```

試著測試以下範別，用瀏覽器觀察：



### 範例 1：取得內容、屬性

```javascript
console.log($("p").html());        // 取得內容
console.log($("p").attr("class")); // 取得 class 屬性的值
```



### 範例 2：更新 style 屬性

```javascript
$("p").css("color", "red");         // 改變文字顏色
$("p").css("font-style", "italic"); // 變斜體
```

以上程式，等同於：

```javascript
jQuery("p").css("color", "red");         // 改變文字顏色
jQuery("p").css("font-style", "italic"); // 變斜體
```



### 範例 3：更新一般屬性

```javascript
$("p").attr("class", "myclass");
$("p").attr("id", "myid");
$("p").attr("style", "font-weight: bold;font-size: 30px;");
```



### 範例 4：取代裡面的內容

```javascript
$("p").html("<span>這是 span 標籤的內容。</span>");
```

比較以下：

```javascript
$("p").text("<span>這是 span 標籤的內容。</span>");
```



### 範例 5：移除元素

```javascript
$("p").remove();
```



### 範例 6：新增元素至某處

```javascript
$("p").append("<span>這是 span 標籤的內容。</span>"); // 裡面的最後面
```

比較：

```javascript
$("p").prepend("<span>這是 span 標籤的內容。</span>"); // 裡面的最前面
```

比較：

```javascript
$("p").after("<span>這是 span 標籤的內容。</span>"); // 同層後面
```

比較：

```javascript
$("p").before("<span>這是 span 標籤的內容。</span>"); // 同層前面
```

