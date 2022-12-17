---
description: 非同步處理技術及 JSON
cover: >-
  https://images.unsplash.com/photo-1669394146501-a8226175c861?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHJhbmRvbXx8fHx8fHx8fDE2NzEyNjk5MjI&ixlib=rb-4.0.3&q=80
coverY: 0
---

# AJAX

在網頁傳輸的資料越來越多的情況之下，過多的檔案交換會造成傳輸上的效率變差。\
AJAX則是解決資料傳輸的一種技術，JSON則是資料格式

#### AJAX 的優點

不更新整個頁面的前提下，僅向伺服器傳送並取回必須的資料，不會造成傳輸過多重複內容\
在網路頻寬不良的狀況下，減少大量資料，提升傳輸速度

#### AJAX - 格式內容 :

> 提AJAX格式之前要先提到 method\
> method 是 瀏覽器送出請求給伺服器的方式，可以想像是現實中的郵差\
> 常用的有兩種
>
> 1. GET : 類似於現實中的明信片，資料的內容會直接顯示在url上。\
>    例如 url:'abc.com?a=1\&b=2'\
>    ?後面的a=1\&b=2就是送出的資料值
> 2. POST : 有別於GET，類似信件或包裹，將資料內容包裝在信封裡面才做發送。\
>    而POST裡面可以包含任意資料或檔案。

1. ulr : 某伺服器提供的服務
2. method : 送出請求的方式 ( GET or POST )
3. dataType : 伺服器回傳的資料型態 ( 如果未指定，會依據瀏覽器會依據型態自行轉換)
4. data : 送出的資料內容 ( 如果使用GET，就不會有這個屬性 ) 可以指定為JSON
5. 資料傳輸成功或失敗時進行的操作(非必要):

> 這裡通常使用函式去對應\
> ex:\
> success:function(res){console.log(res)},\
> error:function(err){console.log(err)}

### JSON

> 是一種資料格式

> JSON的基本資料類型： 數值：十進位數，不能包含非數，如NaN。不區分整數與浮點數。\
> 字串：以""括起來的零個或多個Unicode碼位。支援\開始的跳脫字元序列。\
> 布林值：表示為true或者false。\
> 陣列：有序的零或者多個值。每個值可以為任意類型。\
> 陣列使用方括號\[ ]包裹。多個陣列元素之間用逗號,分隔，形如：\[value1,value2]\
> 物件：無序的 "Key":Value 組成，物件以花括號{ }包裹，Key只能是字串\
> 空值：值寫為null

因為JSON格式內容由屬性和值所組成，因此也有易於閱讀和處理的優勢。\
許多語言都有辦法將JSON的內容進行解析並字串化，已經變成主流的資料傳輸格式
