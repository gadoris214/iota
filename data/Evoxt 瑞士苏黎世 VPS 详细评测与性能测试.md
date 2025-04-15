# Evoxt 瑞士苏黎世 VPS 详细评测与性能测试

## 产品配置与购买信息

本次测试机型为 Evoxt 最新推出的瑞士苏黎世数据中心 VPS，基础配置如下：

- **CPU**: 1 vCore (AMD EPYC-Genoa 处理器)
- **内存**: 512 MB
- **存储**: 5 GB SSD
- **流量**: 500 GB/月
- **价格**: 2.99 美元/月

👉 [【点击查看】2025年最新 Evoxt优惠码及特价云服务器方案汇总](https://bit.ly/evoxt)

## 数据中心与网络概况

Evoxt 瑞士苏黎世数据中心采用新一代 EPYC Genoa 处理器，性能表现优异。测试时 IP 地址仍显示为马来西亚（数据库更新延迟），但实际物理位置位于瑞士苏黎世。

**网络特点**：
- 带宽资源充足
- IPv6 分配为 /48（当前存在部分问题待修复）
- 中国方向网络优化良好

## 详细性能测试数据

### 系统硬件信息

CPU Model Name:        AMD EPYC-Genoa Processor
CPU Cache Size:        L1: 32.00 KB / L2: 1.00 MB / L3: 32.00 MB
Memory Usage:          72.09 MiB / 459.85 MiB
Disk Usage:            2.05 GiB / 4.83 GiB
OS Release:            Debian GNU/Linux 12 (bookworm)
Kernel Version:        6.13.4-x64v3-xanmod1

### 处理器性能

1 Thread(s) Test:      6112.02 Scores (1.00x)

### 磁盘I/O性能

Write Test (4K-Block):     219.30 MB/s (56140 IOPS)
Read Test (4K-Block):      704.22 MB/s (180281 IOPS)
Write Test (128K-Block):   3846.15 MB/s (30769 IOPS)
Read Test (128K-Block):    9090.91 MB/s (72727 IOPS)

## 网络速度测试

### 国际方向 iperf3 结果

| 节点位置           | 发送速度      | 接收速度      |
|--------------------|---------------|---------------|
| 伦敦(10G)         | 3.85 Gbps     | 5.15 Gbps     |
| 阿姆斯特丹(100G)  | 5.15 Gbps     | 3.54 Gbps     |
| 洛杉矶(10G)       | 579 Mbps      | 1.39 Gbps     |

### 中国方向 Speedtest

**中国电信江苏5G节点**:
- 下载: 1484.97 Mbps
- 上传: 631.76 Mbps
- 延迟: 185.11 ms

**中国联通上海5G节点**:
- 下载: 3608.40 Mbps
- 上传: 591.13 Mbps
- 延迟: 200.74 ms

## 流媒体解锁测试

**IPv4解锁情况**:
- Netflix: 支持(马来西亚区)
- Disney+: 即将支持
- YouTube Premium: 支持(马来西亚区)
- Amazon Prime Video: 支持(美国区)
- ChatGPT/Google Gemini/Claude: 全部可用

## 路由追踪分析

### 中国电信(北京)

1  瑞士苏黎世(3.10ms) → 德国法兰克福(9.76ms) → 北京(237.59ms)

### 中国联通(上海)

1  瑞士苏黎世(2.47ms) → 德国法兰克福(9.85ms) → 广州(173.19ms) → 上海(232.85ms)

### 中国移动(广州)

1  瑞士苏黎世(10.07ms) → 德国慕尼黑(6.38ms) → 美国洛杉矶(161.60ms) → 广州(490.76ms)

## 总结评价

Evoxt 瑞士苏黎世 VPS 在性能与价格方面表现出色，特别适合需要欧洲节点的用户。虽然基础配置较小，但可通过升级方案获得更高性能。网络方面对中国方向有良好优化，是性价比极高的海外VPS选择。