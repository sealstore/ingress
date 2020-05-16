# ingress

- [contour](https://github.com/sealstore/ingress/tree/contour) 是基于Envoy实现的ingress controller,不仅支持Ingress还支持IngressRouter，功能更为强大，且Envoy自身的配置发现能力更强，是本人极为推荐的一个Ingress controller.


## 使用方法
注意，请使用sealos最新版本，如果是老版本sealos安装的集群不会自动生成sealos配置文件，需要自己手动配置，会输出日志教你如何配置

本地拉取(先到[release页面](https://github.com/sealstore/ingress/releases)下载好tar包到本地)：
```
wget https://github.com/sealstore/ingress/releases/download/v0.15.2/contour.tar
sealos install --pkg-url contour.tar
```
或者远程拉取：
```
sealos install --pkg-url https://github.com/sealstore/ingress/releases/download/v0.15.2/contour.tar
```
