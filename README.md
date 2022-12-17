# AJAX跟JSON
> 非同步處理技術及資料格式

AJAX的優點
不更新整個頁面的前提下，僅向伺服器傳送並取回必須的資料，不會造成傳輸過多重複內容
在網路頻寬不良的狀況下，減少大量資料，提升傳輸速度

AJAX - 格式內容 :

ulr : 某伺服器提供服務的連結
method : 送出請求的方式
GET
POST
dataType : 
data : 

success:function(res){console.log(res)},
  error:function(err){console.log(err)},