代理池
============

## 注意

本代码库仅用于学习研究使用，请勿用于非法用途，本人不承担由此带来的任何法律问题。

## 介绍

在[《爬虫实战：从数据到产品》](https://item.jd.com/12575102.html)一书中，我讲到了一个基于ProxyBroker的代理池。经过我的长时间的实践，这个代理池用起来非常的方便和稳定。

这个Repo将基于[ProxyBroker](https://github.com/constverum/ProxyBroker)，增加了中国区域的代理资源。并引入了docker-compose，能够快速的方便的开始代理的抓取。

## 用法

```
docker-compose up
```

然后浏览器打开http://localhost:8080/proxy.json 即可得代理列表。每个代理都经过类型的验证，代理资源会随着时间增长。每个代理的有效期为一天时间。

由于很多代理资源在中国无法访问的网站，部署在国内的服务器上会影响资源的获取，所以推荐将服务器部署到国外的服务器。服务器推荐使用[DigitalOcean](https://m.do.co/c/4bc532e3ef94)，我的多个服务器都在SFO2区域，非常的稳定。
