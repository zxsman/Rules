[custom]

;解決DNS洩露，無分流群組
ruleset=🚀 節點選擇,[]DOMAIN-SUFFIX,xn--ngstr-lra8j.com
ruleset=🚀 節點選擇,[]DOMAIN-SUFFIX,services.googleapis.cn
ruleset=🚀 節點選擇,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/GoogleCNProxyIP.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/LocalAreaNetwork.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/UnBan.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaDomain.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaMedia.list
ruleset=REJECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanAD.list
ruleset=REJECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanProgramAD.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaCompanyIp.list
ruleset=DIRECT,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaIp.list
ruleset=DIRECT,[]GEOIP,CN,no-resolve
ruleset=🚀 節點選擇,[]FINAL

custom_proxy_group=🚀 節點選擇`select`[]♻️ 自動選擇`[]DIRECT`.*
custom_proxy_group=♻️ 自動選擇`url-test`.*`http://www.gstatic.com/generate_204`300,,50

enable_rule_generator=true
overwrite_original_rules=true
