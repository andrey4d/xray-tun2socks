# xray-tun2socks for MacOS
### This is a sh-script will route all MacOS traffic through tunnel  tun2socks and xray.

## Run xray as client and tun2sosks 
```shell
./tun2sosks
```
## Install Xray
```shell
brew install xray
```
## Download  tun2socks from https://github.com/xjasonlyu/tun2socks
```sh
curl -L https://github.com/xjasonlyu/tun2socks/releases/download/v2.5.2/tun2socks-darwin-arm64.zip -o tun2socks-darwin-arm64.zip
unzip tun2socks-darwin-arm64.zip
```

## Set TUN2SOCKS variable 
Set TUN2SOCKS variables to access the tune2socks utility by specifying the path

```properties
TUN2SOCKS="/usr/local/bin/tun2socks-darwin-arm64"
```

## Set XRAY_CONFIG variable 
Set XRAY_CONFIG variable specify path to vless_config.json
 ```properties
 XRAY_CONFIG="${HOME}/.vpn/vless_config.json"
 ```


