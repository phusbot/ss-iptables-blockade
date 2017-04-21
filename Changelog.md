## 2017年4月21日

- `新增` FLG.txt新增博讯新闻规则

iptables -I OUTPUT -m string --string "boxunblog.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "peacehall.com" --algo bm -j DROP
