HA-ShadowSocks
==============

Using HA-proxy &amp; multi Sahdowsocks client to make a GFW fucking system.

## 前提

* 已安装haproxy
* 已安装shadowsocks客户端
* 已安装supervisor

## haproxy配置

    sudo ln -sf $项目目录/haproxy/haproxy.cfg /etc/haproxy/haproxy.cfg
    
## supervisor配置

    sudo ln -s $项目目录/supervisor/sslocal.conf /etc/supervisor/conf.d/sslocals.conf 
    sudo supervisorctl update
