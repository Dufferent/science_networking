wget https://install.direct/go.sh
这个是v2ray官方的安装脚本
如果不手动下载v2ray-linux-64.zip
脚本会自动下载，等死呵呵
所以自己下载
我下载好了，放在目录下了嘻嘻
准备好了这两个文件
放在同一目录下
sudo bash go.sh --local ./v2ray-linux-64.zip
执行完成后
配置/etc/v2ray/config.json
怎么配置呢，呵呵
因为我没有国外的vps，也没有订阅过机场之类的v2ray节点
直接去白嫖
******************白嫖有风险哦，说不定哪天就停了，或者网速变慢，又或者信息被窃取（如果你开了全局代理更要小心）********************
贴一个我用的网速挺nice的长期更新的白嫖地址
https://www.butnono.com/latest-2020-freevpn-v2ray-ss-ssr-address.html
这个要梯子，我之前有发过chrom的科学上网插件，随便用一个挂着打开
里面的节点信息用win下的v2ray读取url就能获取到vmess服务器
选中可用的vmess服务器导出客户端配置，就得到了我们需要的config.json(打包好了，但这个服务器不一定长期有效)
好了
sudo systemctl restart v2ray
或者 service ...
或者 /etc/init.d/v2ray ...
随你啦
启动后监听端口10808，这个可以在config.json里修改
这算是完成了，但是你怎么让特定的流量走代理呢
我没那么多时间倒腾
火狐，谷歌浏览器自带的网络设置里可以配置代理贴图在附录里自行查看
做完后
登录youtube
呵呵ok