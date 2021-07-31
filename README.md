
# 自動輸入邀請碼腳本

使用腳本風險自己承擔


### 遊戲中點開活動頁面

![](https://github.com/lightfiretw/TW_LOLanniversaryEvent/blob/main/images/1.png)

### 使用Chrome打開網頁

![](https://github.com/lightfiretw/TW_LOLanniversaryEvent/blob/main/images/2.png)

### F12輸入腳本

```
if(localStorage.getItem("ingame-token")!=null){var s = "var yourToken=\""+localStorage.getItem("ingame-token")+"\";fetch(\"https://raw.githubusercontent.com/lightfiretw/TW_LOLanniversaryEvent/main/ID_json\").then(e=>e.json()).then(e=>e.id).then(e=>{e.forEach((e,n)=>{setTimeout(function(){console.log(n),fetch(\"https://bargain.lol.garena.tw/api/enter\",{method:\"POST\",body:JSON.stringify({code:e,confirm:!0}),headers:{Token:yourToken,\"Content-Type\":\"application/json\"}})},1e6*n)})});";copy(s);this.document.location="https://bargain.lol.garena.tw/api/enter";}else{alert("請從LOL開啟活動網頁")}
```

![](https://github.com/lightfiretw/TW_LOLanniversaryEvent/blob/main/images/3.png)


## 直接在新畫面CTRL+V


![](https://github.com/lightfiretw/TW_LOLanniversaryEvent/blob/main/images/4.png)


## 忽略出錯

![](https://github.com/lightfiretw/TW_LOLanniversaryEvent/blob/main/images/5.png)

