# v2raya

## 一、前提条件

⚠️ **必须使用虚拟机（VM）或实体机**

- ✅ PVE KVM 虚拟机
- ✅ 裸机 / 物理服务器
- ❌ **不支持 PVE CT（LXC）**
- ❌ 不支持容器型 VPS（OpenVZ / LXC）

原因：
- v2raya 的透明代理 / 网关模式需要修改内核网络（iptables / TPROXY）
- CT / LXC 没有完整内核权限

## 二、安装 v2raya

### 1️⃣ 拉取镜像
    docker pull mzz2017/v2raya


## 运行容器（网关 / 透明代理模式）
    docker run -d \
      --restart=always \
      --privileged \
      --network=host \
      --name v2raya \
      -e V2RAYA_LOG_FILE=/tmp/v2raya.log \
      -e V2RAYA_V2RAY_BIN=/usr/local/bin/v2ray \
      -e V2RAYA_NFTABLES_SUPPORT=off \
      -e IPTABLES_MODE=legacy \
      -v /lib/modules:/lib/modules:ro \
      -v /etc/resolv.conf:/etc/resolv.conf \
      -v /etc/v2raya:/etc/v2raya \
      mzz2017/v2raya
## 访问
    http://<服务器IP>:2017


## 启用透明代理 / 系统代理
-  透明代理 / 系统代理：✅ 启用

-  代理模式：大陆白名单模式

-  实现方式：redirect

-  规则端口的分流模式：大陆白名单模式

-  防止 DNS 污染：✅ 转发 DNS 请求
