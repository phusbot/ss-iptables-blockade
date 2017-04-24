## 2017年4月24日

- `新增` China.txt新增百度规则

iptables -I OUTPUT -m string --string "tieba.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "bdstatic.cn" --algo bm -j DROP

iptables -I OUTPUT -m string --string "duapp.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "dwz.cn" --algo bm -j DROP

iptables -I OUTPUT -m string --string "skycn.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "qianqian.com" --algo bm -j DROP

## 2017年4月22日

- `新增` FLG.txt新增博讯论坛规则

iptables -I OUTPUT -m string --string "boxunclub.com" --algo bm -j DROP

## 2017年4月21日

- `新增` FLG.txt新增博讯新闻规则

iptables -I OUTPUT -m string --string "boxunblog.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "peacehall.com" --algo bm -j DROP
