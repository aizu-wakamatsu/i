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
起動直後にenter
```
apboot> setenv ipaddr ___.___.___.___
apboot> setenv netmask ___.___.___.___
apboot> setenv gatewayip ___.___.___.___  
apboot> setenv dnsip ___.___.___.___
apboot> setenv name <hostname>
apboot> saveenv
apboot> boot
```

# Uplink WLAN
```
(Instant AP)(config) # wlan sta-profile
(Instant AP)(sta uplink)# cipher-suite <clear | wpa-tkip-psk | wpa2-ccmp-psk | wpa3-sae-aes>
(Instant AP)(sta uplink)# essid <essid>
(Instant AP)(sta uplink)# uplink-band <dot11a/dot11g/dot116GHz>
(Instant AP)(sta uplink)# wpa-passphrase <key>
```


# 参考リンク
https://arubanetworking.hpe.com/techdocs/Instant_8.x_WebHelp/Content/instant-ug/uplink-conf/wifi-uplink.htm
https://invisibletechnology.jp/aruba-instant-ap-setting/#toc5