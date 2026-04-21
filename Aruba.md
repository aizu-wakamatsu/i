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
## 構成
```
(Instant AP) # config
(Instant AP)(config) # wlan sta-profile
(Instant AP)(sta uplink)# cipher-suite <clear | wpa-tkip-psk | wpa2-ccmp-psk | wpa3-sae-aes>
(Instant AP)(sta uplink)# essid <essid>
(Instant AP)(sta uplink)# uplink-band <dot11a/dot11g/dot116GHz>
(Instant AP)(sta uplink)# wpa-passphrase <key>
(Instant AP)(sta uplink) # exit
(Instant AP)(config) # exit
(Instant AP) #
```
## 設定の確認
```
(Instant AP)# show wifi-uplink status
```
## ステータスの確認
```
(Instant AP)# show wifi-uplink config
```

# 参考リンク
https://arubanetworking.hpe.com/techdocs/Instant_8.x_WebHelp/Content/instant-ug/uplink-conf/wifi-uplink.htm
https://invisibletechnology.jp/aruba-instant-ap-setting/#toc5
https://arubanetworking.hpe.com/techdocs/Instant_8.x_WebHelp/Content/instant-ug/uplink-conf/uplink-mgmt.htm#Enforcin
https://arubanetworking.hpe.com/techdocs/InstantWenger_Mobile/Advanced/Content/Instant%20User%20Guide%20-%20volumes/Ethernet_Downlink.htm