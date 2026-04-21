# シリアルポートの設定

|              |      |
| ------------ | ---- |
| Baud rate    | 9600 |
| Data         | 8bit |
| Parity       | none |
| Stop         | 1bit |
| Flow control | none |
|              |      |
|              |      |
|              |      |
# apbootコマンド
```
apboot> setenv ipaddr ___.___.___.___
apboot> setenv netmask ___.___.___.___
apboot> setenv gatewayip ___.___.___.___  
apboot> setenv dnsip ___.___.___.___
apboot> setenv name <hostname>
apboot> saveenv
apboot> boot
```




# 参考リンク
https://invisibletechnology.jp/aruba-instant-ap-setting/#toc5