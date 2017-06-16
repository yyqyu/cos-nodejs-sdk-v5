# cos-nodejs-sdk-v5

腾讯云 COS Nodejs SDK（[XML API](https://www.qcloud.com/document/product/436/7751)）

[releases](https://github.com/tencentyun/cos-nodejs-sdk-v5/releases)

## 使用文档

https://www.qcloud.com/document/product/436/8629

## npm 安装

 [npm 地址](https://www.npmjs.com/package/cos-nodejs-sdk-v5)
 
```
npm i cos-nodejs-sdk-v5 --save
```

## get started

```javascript
var COS = require('cos-nodejs-sdk-v5');
var cos = new COS({
    AppId: '1253669060 ',
    SecretId: 'AKIDvlRzPfuePCuTr5O0hDYihU7f7PWSP0Ws',
    SecretKey: 'KUTH0b1SnxxmQtCLK9nGYfbM2ax9A1iI',

});
// 分片上传
cos.sliceUploadFile({
    Bucket: 'test',
    Region: 'cn-south',
    Key: '1.zip',
    FilePath: './1.zip'
}, function (err, data) {
    console.log(err, data);
});
```
