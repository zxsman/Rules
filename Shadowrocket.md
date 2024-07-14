# Shadowrocket配置文件，解決DNS洩漏
[General]<br>
bypass-system = true<br>
skip-proxy = 192.168.0.0/16, 10.0.0.0/8, 172.16.0.0/12, localhost, *.local, captive.apple.com<br>
tun-excluded-routes = 10.0.0.0/8, 100.64.0.0/10, 127.0.0.0/8, 169.254.0.0/16, 172.16.0.0/12, 192.0.0.0/24, 192.0.2.0/24, 192.88.99.0/24, 192.168.0.0/16, 198.51.100.0/24, 203.0.113.0/24, 224.0.0.0/4, 255.255.255.255/32, 239.255.255.250/32<br>
dns-server = system<br>
ipv6 = false<br>
prefer-ipv6 = false<br>
dns-fallback-system = false<br>
dns-direct-system = false<br>
icmp-auto-reply = true<br>
always-reject-url-rewrite = false<br>
private-ip-answer = true<br>
dns-direct-fallback-proxy = true<br>

[Rule]<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/LocalAreaNetwork.list,DIRECT<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/UnBan.list,DIRECT<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaDomain.list,DIRECT<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaMedia.list,DIRECT<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanAD.list,REJECT<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanProgramAD.list,REJECT<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaCompanyIp.list,DIRECT<br>
RULE-SET,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaIp.list,DIRECT<br>
GEOIP,CN,DIRECT,no-resolve<br>
FINAL,PROXY<br>

[Host]<br>
localhost = 127.0.0.1<br>

[URL Rewrite]<br>
^https?://(www.)?g.cn https://www.google.com 302<br>
^https?://(www.)?google.cn https://www.google.com 302<br>
