# ouster雷达安装

## 1.0 设置静态ip

 ### 1.1 查看雷达当前的ip

```
# 指令：ping -c3 os-[ouster码]如下图
# 比如：
$ ping -c3 os-992112000030
PING os-992112000030.local (169.254.214.51) 56(84) bytes of data.
From neousys-Nuvo-6108GC (10.10.1.149) icmp_seq=1 Destination Host Unreachable
From neousys-Nuvo-6108GC (10.10.1.149) icmp_seq=2 Destination Host Unreachable
From neousys-Nuvo-6108GC (10.10.1.149) icmp_seq=3 Destination Host Unrechable
# 现在雷达ip为：10.10.1.149
```

<img src="..\picture\sensor_install\ouster码.png" style="zoom:60%;" />

## 1.2 设置ouster静态ip

```
# 约定：ouster静态雷达ip统一设置为：192.168.1.117
```

具体详细查看：https://os.twty.net/#/staticIP

## 1.3 查看雷达当前的ip

```
$ ping -c3 os-992112000030.local
PING os-992112000030.local (192.168.1.117) 56(84) bytes of data.
64 bytes from 192.168.1.117 (192.168.1.117): icmp_seq=1 ttl=64 time=0.339 ms
64 bytes from 192.168.1.117 (192.168.1.117): icmp_seq=2 ttl=64 time=0.194 ms
64 bytes from 192.168.1.117 (192.168.1.117): icmp_seq=3 ttl=64 time=0.199 ms
# 现在雷达ip为：192.168.1.117
```

## 1.4 ouster的IP设置成功