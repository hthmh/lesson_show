[source](https://juejin.im/post/5b01336af265da0b8a67e5c9)

反向代理   负载均衡

服务器集群， 每台服务器的内容一样时，从个人电脑访问服务器时无法访问， 通过第三方服务器才能访问集群。

并不知道是哪一台服务器提供的内容， 代理方式称为反向代理。

负载均衡
先访问一个中间服务器， 在服务器中选择一个压力较小的服务器， 然后将该访问请求引入选择的服务器。

nginx 会给你分配服务器压力小的去访问

反向代理
proxy_pass

Upstream 模块实现负载均衡
ip_hash 指令
server 指令
upstream 指令及相关变量