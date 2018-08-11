## 2018年8月11日

- `创建` China.txt创建抖音、开发SDK、小蚁规则

- `修改` China.txt修改站长统计规则

iptables -I OUTPUT -m string --string "umeng.com" --algo bm -j DROP

修改为

iptables -I OUTPUT -m string --string "umeng" --algo bm -j DROP

- `新增` China.txt新增IP查询规则

iptables -I OUTPUT -m string --string "ip-api.com" --algo bm -j DROP

- `新增` 广告&统计规则

iptables -I OUTPUT -m string --string "flurry.com" --algo bm -j DROP

- `新增` 搜狐规则

iptables -I OUTPUT -m string --string "sogoucdn.com" --algo bm -j DROP

- `新增` 网易规则

iptables -I OUTPUT -m string --string "netease.im" --algo bm -j DROP

iptables -I OUTPUT -m string --string "qiyukf.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "yixin.im" --algo bm -j DROP

- `新增` 阿里巴巴规则

iptables -I OUTPUT -m string --string "alipayobjects.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "aliyuncs.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "dingtalk.com" --algo bm -j DROP

iptables -I OUTPUT -m string --string "mybank.cn" --algo bm -j D

## 2018年5月12日

- `新增` China.txt新增小米规则

iptables -I OUTPUT -m string --string "miui.com" --algo bm -j DROP

- `新增` 360规则

iptables -I OUTPUT -m string --string "360kan.com" --algo bm -j DROP

## 2017年11月14日

- `新增` China.txt新增网易规则

iptables -I OUTPUT -m string --string "126.net" --algo bm -j DROP

- `新增` 新浪&微博规则

iptables -I OUTPUT -m string --string "sina.com.hk" --algo bm -j DROP

iptables -I OUTPUT -m string --string "sina.com.tw" --algo bm -j DROP

## 2017年11月9日

- `创建` China.txt创建知乎规则

iptables -I OUTPUT -m string --string "zhihu.com" --algo bm -j DROP

## 2017年8月25日

- `创建` China.txt创建政府规则

iptables -I OUTPUT -m string --string "gov.cn" --algo bm -j DROP

## 2017年5月5日

- `修改` Stop.txt修改疑似蜜罐规则

iptables -I OUTPUT -m string --string "rixcloud.com" --algo bm -j DROP

修改为

iptables -I OUTPUT -m string --string "rixcloud" --algo bm -j DROP

## 2017年5月4日

- `创建` China.txt创建堆糖、蘑菇街、美丽说规则

- `创建` Stop.txt创建规则

## 2017年4月26日

- `新增` China.txt新增腾讯规则

iptables -I OUTPUT -m string --string "qpic.cn" --algo bm -j DROP

iptables -I OUTPUT -m string --string "gtimg.cn" --algo bm -j DROP

iptables -I OUTPUT -m string --string "url.cn" --algo bm -j DROP

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
