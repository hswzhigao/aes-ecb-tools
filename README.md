# AES ECB 加解密工具

## 在线地址

https://dcfdf54d.pinme.dev

## 功能

- 左侧：输入 enc.key 和明文，点击加密，生成 Base64 密文，支持复制
- 右侧：输入 enc.key 和密文，点击解密，得到明文，支持复制
- 加密次数、解密次数分别计数，使用 localStorage 持久化
- 所有计算在浏览器本地完成，不发送到服务器

## 与 Java 端互通

使用 AES/ECB/PKCS5Padding + Base64，与 hire-server 的 `AesEcbUtils.encryptWithoutIv / decryptWithoutIv` 完全互通。

## 本地文件

`index.html` — 单文件，零框架，使用 CryptoJS CDN
