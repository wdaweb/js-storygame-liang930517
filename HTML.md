**上傳圖片**
`<form action="" method="" enctype="multipart/form-data">` enctype一定要寫

**上傳檔案**
`<form method="post"...` 上傳檔案必須用"post"接住

## 關於CSS height高度屬性

1. height:100%
如果在一個div設置一張背景圖，並設置width:100% ;hight:100% ，
會發現div的高度根本稱不開。這時需在CSS設定
```html
html,
body{
    height:100%;
}
```
**因為height的百分比值需要父級有一個可以生效的高度值才起作用。**

1. height:100vh
vh(view height)指瀏覽器內部的可視區域高度的百分比，window.innerWidth/window.innerHeight
上述例子問題也可以使用vh單位解決，不用在html，body上設hight:100%
但是vh單位在IE8以下版本不支援。