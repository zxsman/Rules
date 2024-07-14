# https://cf.buliang0.cf/clash-rules/nodnsleak.ini
[custom]<br>
;解決DNS洩露，無分流群組<br>
ruleset=🚀 節點選擇,[]DOMAIN-SUFFIX,xn--ngstr-lra8j.com<br>
ruleset=🚀 節點選擇,[]DOMAIN-SUFFIX,services.googleapis.cn<br>
ruleset=🚀 節點選擇,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/GoogleCNProxyIP.list<br>
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/LocalAreaNetwork.list<br>
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/UnBan.list<br>
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaDomain.list<br>
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaMedia.list<br>
ruleset=REJECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanAD.list<br>
ruleset=REJECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanProgramAD.list<br>
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaCompanyIp.list<br>
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaIp.list<br>
ruleset=DIRECT,[]GEOIP,CN,no-resolve<br>
ruleset=🚀 節點選擇,[]FINAL<br>

custom_proxy_group=🚀 節點選擇`select`[]♻️ 自動選擇`[]DIRECT`.*<br>
custom_proxy_group=♻️ 自動選擇`url-test`.*`http://www.gstatic.com/generate_204`300,,50<br>

enable_rule_generator=true<br>
overwrite_original_rules=true<br>
