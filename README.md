這是一個簡單輕巧的Parse Spreadsheet的工具

> 本專案有用 `$.ajax(...)` 請務必於連結於 `jQuery` 之後

```html
  
  ...

  <script src="/path/to/jquery.js"></script>
  <script src="/path/to/spreadsheetSoup.js"></script>
  
  ...

```

你也可以直接用gh-pages當作script連結

```html

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.0.0-alpha1/jquery.min.js"></script>
  <script src="http://qas612820704.github.io/spreadsheetSoup/spreadsheetSoup.js"></script>

```

該怎麼用?

```js

  // function SpreadsheetSoup(key, sheet, callbackSucess, callbackError) { ... };

  // 官方的範例 key就是你的Spreadsheets
  var key = 'o13394135408524254648.240766968415752635'
  var sheet = '1'
  
  function mySuccess(data) {
    console.log(data);
  };

  function myErr(data) {
    console.log(data);
  }

  var soup = new SpreadsheetSoup(key, sheet, mySuccess, myErr);

```

 Output :
```
  [Object, Object, Object, Object, Object, Object, Object, Object]

  0:
    Objecthours: "10"
    ipm: "0.003333333333"
    items: "2"
    name: "Bingley"
    __proto__: Object
  1:
    Objecthours: "200"
    ipm: "6.28"
    items: "75360"
    name: "Captain Carter"
    __proto__: Object
  2:
    Objecthours: "200"
    ipm: "8.333333333"
    items: "100000"
    name: "Dawson"
    __proto__: Object
  3:
    Objecthours: "40"
    ipm: "0.01666666667"
    items: "40"
    name: "Colonel Forster"
    __proto__: Object
  4:
    Objecthours: "100"
    ipm: "4.307"
    items: "25842"
    name: "William Goulding"
    __proto__: Object
  5:
    Objecthours: "100"
    ipm: "4.278333333"
    items: "25670"
    name: "Lady Lucas"
    __proto__: Object
  6:
    Objecthours: "190"
    ipm: "8.663596491"
    items: "98765"
    name: "Sir William"
    __proto__: Object
  7:
    Objecthours: "60"
    ipm: "5"i
    tems: "18000"
    name: "Charlotte"
    __proto__: Object
  length: 8__proto__: Array[0]

```

簡單且漂亮的輸出 而且檔案也非常小(大概40行XD)

希望大家喜歡
