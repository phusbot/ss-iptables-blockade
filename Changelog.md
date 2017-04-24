## 2017年4月24日

- `新增` China.txt新增百度、千千静听、糯米规则

iptables -I OUTPUT -m string --string "tieba.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "bdstatic.cn" --algo bm -j DROP

iptables -I OUTPUT -m string --string "duapp.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "dwz.cn" --algo bm -j DROP

iptables -I OUTPUT -m string --string "skycn.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "qianqian.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "baidustatic.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "baidupcs.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "hao123.net" --algo bm -j DROP

iptables -I OUTPUT -m string --string "nuomi.com" --algo bm -j DROP

- `新增` 腾讯规则

iptables -I OUTPUT -m string --string "wegame.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "qcloud.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "qplus.com" --algo bm -j DROP

- `新增` 阿里巴巴规则

iptables -I OUTPUT -m string --string "aliyun.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "alitrip.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "fliggy.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "alibaba.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "1688.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "yunos.com" --algo bm -j DROP

- `创建` 携程规则

- `创建` 映客规则

## 2017年4月22日

- `新增` FLG.txt新增博讯论坛规则

iptables -I OUTPUT -m string --string "boxunclub.com" --algo bm -j DROP

## 2017年4月21日

- `新增` FLG.txt新增博讯新闻规则

iptables -I OUTPUT -m string --string "boxunblog.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "peacehall.com" --algo bm -j DROP
