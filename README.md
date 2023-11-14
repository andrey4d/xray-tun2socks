# xray-tun2socks for MacOS
### This is a sh-script will route all MacOS traffic through tunnel  tun2socks and xray.

## Run xray as client and tun2sosks 
```shell
./tun2sosks
```

# Requirements  
## Install Xray
```shell
brew install xray
```
## Download  tun2socks
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

## Example
```text
user@mbook:github/xray-tun2socks ‹main›$ ./tun2socks
Server IP 182.125.18.196
Default gateway 192.168.1.1
Run xray.
Run tun2socks to localhost:1080
add route 182.125.18.196/32 to 172.16.0.1.
add route 1.0.0.0/8 to 172.16.0.1.
add route 2.0.0.0/7 to 172.16.0.1.
add route 4.0.0.0/6 to 172.16.0.1.
add route 8.0.0.0/5 to 172.16.0.1.
add route 16.0.0.0/4 to 172.16.0.1.
add route 32.0.0.0/3 to 172.16.0.1.
add route 64.0.0.0/2 to 172.16.0.1.
add route 128.0.0.0/1 to 172.16.0.1.
Xray 1.8.4 (Xray, Penetrates Everything.) Custom (go1.21.0 darwin/arm64)
A unified platform for anti-censorship.
2023/11/14 16:57:16 [Info] infra/conf/serial: Reading config: /Users/andrey/.vpn/vless_config.json
2023/11/14 16:57:30 tcp:[::1]:55029 accepted tcp:152.251.44.16:443 [in_proxy >> proxy]
2023/11/14 16:57:30 tcp:[::1]:55028 accepted tcp:152.251.44.16:443 [in_proxy >> proxy]
2023/11/14 16:57:30 tcp:[::1]:55026 accepted tcp:152.251.44.16:443 [in_proxy >> proxy]
2023/11/14 16:57:30 tcp:[::1]:55025 accepted tcp:152.251.44.16:443 [in_proxy >> proxy]
2023/11/14 16:57:30 tcp:[::1]:55027 accepted tcp:152.251.44.16:443 [in_proxy >> proxy]
2023/11/14 16:57:30 tcp:[::1]:55024 accepted tcp:152.251.44.16:443 [in_proxy >> proxy]
^C** Trapped CTRL-C
delete route 182.125.18.196/32 to 172.16.0.1.
delete route 1.0.0.0/8 to 172.16.0.1.
delete route 2.0.0.0/7 to 172.16.0.1.
delete route 4.0.0.0/6 to 172.16.0.1.
delete route 8.0.0.0/5 to 172.16.0.1.
delete route 16.0.0.0/4 to 172.16.0.1.
delete route 32.0.0.0/3 to 172.16.0.1.
delete route 64.0.0.0/2 to 172.16.0.1.
delete route 128.0.0.0/1 to 172.16.0.1.
Done.
```

## :octocat: Credits

https://github.com/xjasonlyu/tun2socks

https://github.com/XTLS/Xray-install

https://github.com/iamtrazy/xray-tun2socks
