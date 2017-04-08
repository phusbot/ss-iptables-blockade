# 一个基于iptables的“非法访问”封锁列表。

项目建立缘由百度系列APP和内置百度API的APP未经用户许可，私自收集用户精确地理位置并与IP地址进行绑定（收集也包括境外VPS的IP地址），并生成大数据供开发者使用（当然也可能包括政府），造成的后果是，查询你境外私有的科学上网服务器的IP地址会定位到你经常科学上网的地方，例如你家地址。VPS的IP地址被百度收集，大部分原因是用户设置不当造成的，其中包括使用了全局代理。当然并不止百度会收集这些数据，高德、腾讯、阿里巴巴、京东等都会收集这些数据。

项目的建立是防止这类收集事件的发生，但是世界之大，无奇不有，屏蔽是屏蔽不完的，项目目前只收录常见的域名，小众的域名你可以在Telegram社群里面反馈，防止这类事件的发生就应该选择gfwlist模式，而不是全局模式。

————

## 收录名单

China.txt 收录屏蔽国内常见域名

World.txt 收录屏蔽国外常见域名

FLG.txt 收录屏蔽法轮功常见域名

Green.txt 收录放行国外常见域名

屏蔽：无法使用本服务器访问的网站和APP。
放行：因屏蔽规则造成国外正常服务无法访问的解决规则。

————

## 使用方法

1.SSH登录VPS

2.复制粘贴规则回车

3.将添加的规则保存到文件

iptables-save > /etc/iptables

4.添加自启动

vi /etc/network/interfaces

填入以下规则

pre-up iptables-restore < /etc/iptables

保存

————

## 常见问题

- Q 为什么国内常见域名会包含华为、vivo、oppo、触宝等这些域名？

  A 因为国产手机内置了删不掉的厂商官方应用和第三方应用。
  
- Q 有些不常见的域名是哪里得来的？

  A 都是通过抓包得出来的地址。
  
- Q 我自己如何增加删减规则？

  A 增加
  
    iptables -I OUTPUT -m string --string "增加屏蔽的网址" --algo bm -j DROP
    
    iptables -I OUTPUT -m string --string "增加放行的网址" --algo bm -j ACCEPT
    
    删除
    
    iptables -D OUTPUT -m string --string "删除屏蔽的网址" --algo bm -j DROP
    
    iptables -D OUTPUT -m string --string "删除放行的网址" --algo bm -j ACCEPT
    
    就这么简单
    
    -I 是插入iptables规则；
    
    -D 是删除对应的iptables规则；
    
    -j DROP 是丢弃数据包；
    
    -j ACCEPT 是接受数据包。
    
    如果你有规则，希望你乐意分享。
