# digitalocean-benchmark

## bash

```bash
uname -r
echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf
sysctl -p
lsmod | grep bbr

wget -qO- bench.sh | bash

bash <(curl -sSL "https://git.io/JswGm")

bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
```

all results are form DO-Premium-AMD 1H1G

## 旧金山 143.198.137.97

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1996.250 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (145.6 MB Used)
 System uptime      : 0 days, 0 hour 5 min
 Load average       : 1.19, 0.55, 0.22
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : cubic
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : Santa Clara / US
 Region             : California
----------------------------------------------------------------------
 I/O Speed(1st run) : 899 MB/s
 I/O Speed(2nd run) : 789 MB/s
 I/O Speed(3rd run) : 758 MB/s
 I/O Speed(average) : 518.0 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1992.55 Mbps      9052.91 Mbps        166.61 ms
```

```bash
- IPV4 -
 IP:                                    143.198.137.97
 Country:                               United States
 Region:                                California
 City:                                  Santa Clara
 ISP:                                   DigitalOcean, LLC
 Org:                                   DigitalOcean, LLC

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               Yes
 HBO Max:                               No
 Paramount+:                            Yes
 Peacock TV:                            Yes
 Sling TV:                              Yes
 Pluto TV:                              Yes
 encoreTVB:                             Failed
 ABC:                                   No

 -- Europe --
 BritBox:                               Yes
 ITV Hub:                               No
 Channel 4:                             No
 BBC iPLAYER:                           No
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: US)
 Amazon Prime Video:                    Yes(Region: US)
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: US)
 Viu.com:                               No
 Steam:                                 Yes(Currency: USD)
```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 120.81    ↓ 5715.45   134.34  
17145 电信|安徽合肥５Ｇ　　↑ 128.79    ↓ 3352.10   145.27  
27594 电信|广东广州５Ｇ　　↑ 24.79     ↓ 1230.18   186.46  
5396  电信|江苏苏州５Ｇ　　↑ 576.20    ↓ 3640.39   140.19  
23844 电信|湖北武汉　　　　↑ 5.27      ↓ 262.74    159.56  
29353 电信|湖北武汉５Ｇ　　↑ 15.29     ↓ 204.66    199.49  
28225 电信|湖南长沙５Ｇ　　↑ 223.30    ↓ 1840.07   167.68  
3973  电信|甘肃兰州　　　　↑ 3.85      ↓ 43.15     163.86  
24447 联通|上海５Ｇ　　　　↑ 336.34    ↓ 4349.01   173.42  
27154 联通|天津５Ｇ　　　　↑ 328.57    ↓ 4420.73   154.25  
13704 联通|江苏南京　　　　↑ 151.98    ↓ 1236.13   191.29  
4870  联通|湖南长沙　　　　↑ 288.00    ↓ 810.22    178.96  
25858 移动|北京　　　　　　↑ 422.20    ↓ 4012.76   195.04  
16398 移动|贵州贵阳　　　　↑ 370.49    ↓ 3710.23   204.08  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 7 分 40 秒
  当前时间: 2022-03-25 07:01:18
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```
## 纽约 134.122.31.48
```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1999.994 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (139.2 MB Used)
 System uptime      : 0 days, 0 hour 5 min
 Load average       : 0.01, 0.15, 0.09
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : cubic
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : North Bergen / US
 Region             : New Jersey
----------------------------------------------------------------------
 I/O Speed(1st run) : 362 MB/s
 I/O Speed(2nd run) : 743 MB/s
 I/O Speed(3rd run) : 944 MB/s
 I/O Speed(average) : 683.0 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1994.13 Mbps      6833.74 Mbps        0.68 ms
```

```bash
 - IPV4 -
 IP:                                    134.122.31.48
 Country:                               United States
 Region:                                New Jersey
 City:                                  North Bergen
 ISP:                                   DigitalOcean, LLC
 Org:                                   DigitalOcean, LLC

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               Yes
 HBO Max:                               No
 Paramount+:                            Yes
 Peacock TV:                            Yes
 Sling TV:                              Yes
 Pluto TV:                              Yes
 encoreTVB:                             Failed
 ABC:                                   No

 -- Europe --
 BritBox:                               Yes
 ITV Hub:                               No
 Channel 4:                             No
 BBC iPLAYER:                           No
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: US)
 Amazon Prime Video:                    Yes(Region: US)
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: US)
 Viu.com:                               No
 Steam:                                 Yes(Currency: USD)
```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
17145 电信|安徽合肥５Ｇ　　↑ 98.18     ↓ 1260.64   301.90  
27594 电信|广东广州５Ｇ　　↑ 17.96     ↓ 301.34    331.35  
5396  电信|江苏苏州５Ｇ　　↑ 362.22    ↓ 780.73    310.24  
23844 电信|湖北武汉　　　　↑ 10.90     ↓ 963.08    250.78  
29353 电信|湖北武汉５Ｇ　　↑ 5.65      ↓ 1757.63   229.26  
28225 电信|湖南长沙５Ｇ　　↑ 132.11    ↓ 1057.50   246.40  
3973  电信|甘肃兰州　　　　↑ 1.02      ↓ 19.57     277.39  
24447 联通|上海５Ｇ　　　　↑ 209.65    ↓ 265.31    345.11  
27154 联通|天津５Ｇ　　　　↑ 131.49    ↓ 409.09    307.57  
13704 联通|江苏南京　　　　↑ 37.26     ↓ 14.11     323.88  
4870  联通|湖南长沙　　　　↑ 86.68     ↓ 143.95    345.97  
25858 移动|北京　　　　　　↑ 326.11    ↓ 3208.16   248.22  
16398 移动|贵州贵阳　　　　↑ 261.35    ↓ 2746.27   295.82  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 7 分 51 秒
  当前时间: 2022-03-25 07:03:17
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```


## 阿姆斯特丹 188.166.40.36
```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1999.998 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (136.8 MB Used)
 System uptime      : 0 days, 0 hour 2 min
 Load average       : 0.05, 0.06, 0.02
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : bbr
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : Amsterdam / NL
 Region             : North Holland
----------------------------------------------------------------------
 I/O Speed(1st run) : 1.0 GB/s
 I/O Speed(2nd run) : 1.1 GB/s
 I/O Speed(3rd run) : 1.2 GB/s
 I/O Speed(average) : 1126.4 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1995.07 Mbps      16197.73 Mbps       0.23 ms
```


```bash
###############################################################
#  流解锁测试 StreamUnlockTest
#  当前版本: v1.2.2
#  开源地址: https://github.com/LovelyHaochi/StreamUnlockTest
###############################################################
#  国家代码对照表: http://www.loglogo.com/front/countryCode/
#  测试时间: Fri Mar 25 07:16:00 UTC 2022
###############################################################
正在更新软件包列表...
正在安装依赖: jq

- IPV4 -
 IP:                                    188.166.40.36
 Country:                               Netherlands
 Region:                                North Holland
 City:                                  Amsterdam
 ISP:                                   DigitalOcean, LLC
 Org:                                   Digital Ocean

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               No
 HBO Max:                               No
 Paramount+:                            No
 Peacock TV:                            No
 Sling TV:                              No
 Pluto TV:                              Yes
 encoreTVB:                             No
 ABC:                                   No

 -- Europe --
 BritBox:                               No
 ITV Hub:                               No
 Channel 4:                             No
 BBC iPLAYER:                           No
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: NL)
 Amazon Prime Video:                    Yes(Region: NL)
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: INTL)
 Viu.com:                               No
 Steam:                                 Yes(Currency: EUR)
```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 57.79     ↓ 1155.30   277.19  
17145 电信|安徽合肥５Ｇ　　↑ 59.70     ↓ 1512.61   271.12  
27594 电信|广东广州５Ｇ　　↑ 4.44      ↓ 12.67     260.00  
5396  电信|江苏苏州５Ｇ　　↑ 325.04    ↓ 643.41    230.95  
23844 电信|湖北武汉　　　　↑ 30.80     ↓ 392.30    259.98  
29353 电信|湖北武汉５Ｇ　　↑ 60.91     ↓ 40.21     260.90  
28225 电信|湖南长沙５Ｇ　　↑ 77.87     ↓ 31.38     269.33  
3973  电信|甘肃兰州　　　　↑ 4.57      ↓ 20.81     292.54  
24447 联通|上海５Ｇ　　　　↑ 267.03    ↓ 573.43    264.43  
27154 联通|天津５Ｇ　　　　↑ 62.52     ↓ 395.41    336.36  
13704 联通|江苏南京　　　　↑ 10.30     ↓ 8.44      325.86  
4870  联通|湖南长沙　　　　↑ 127.16    ↓ 113.34    356.19  
25858 移动|北京　　　　　　↑ 263.63    ↓ 2743.29   290.18  
16398 移动|贵州贵阳　　　　↑ 309.26    ↓ 3074.87   259.70  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 8 分 19 秒
  当前时间: 2022-03-25 07:26:09
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```

## 新加坡 68.183.224.193
```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1999.998 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (135.6 MB Used)
 System uptime      : 0 days, 0 hour 2 min
 Load average       : 0.17, 0.18, 0.08
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : bbr
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : Singapore / SG
 Region             : Singapore
----------------------------------------------------------------------
 I/O Speed(1st run) : 901 MB/s
 I/O Speed(2nd run) : 1.1 GB/s
 I/O Speed(3rd run) : 1.1 GB/s
 I/O Speed(average) : 1051.3 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1616.31 Mbps      14287.31 Mbps       0.34 ms     
```


```bash
###############################################################
#  流解锁测试 StreamUnlockTest
#  当前版本: v1.2.2
#  开源地址: https://github.com/LovelyHaochi/StreamUnlockTest
###############################################################
#  国家代码对照表: http://www.loglogo.com/front/countryCode/
#  测试时间: Fri Mar 25 07:15:59 UTC 2022
###############################################################
正在更新软件包列表...
正在安装依赖: jq

- IPV4 -
 IP:                                    68.183.224.193
 Country:                               Singapore
 Region:                                ->
 City:                                  Singapore
 ISP:                                   DigitalOcean, LLC
 Org:                                   DigitalOcean, LLC

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               No
 HBO Max:                               No
 Paramount+:                            No
 Peacock TV:                            No
 Sling TV:                              No
 Pluto TV:                              No
 encoreTVB:                             No
 ABC:                                   No

 -- Europe --
 BritBox:                               No
 ITV Hub:                               No
 Channel 4:                             No
 BBC iPLAYER:                           No
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: SG)
 Amazon Prime Video:                    Yes(Region: SG)
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: SG)
 Viu.com:                               Yes(Region: SG)
 Steam:                                 Yes(Currency: SGD)

```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 7.56      ↓ 1.22      258.65  
27594 电信|广东广州５Ｇ　　↑ 8.39      ↓ 10.89     252.10  
24447 联通|上海５Ｇ　　　　↑ 731.94    ↓ 2061.85   117.13  
27154 联通|天津５Ｇ　　　　↑ 363.05    ↓ 2060.08   134.38  
13704 联通|江苏南京　　　　↑ 645.54    ↓ 1281.91   114.68  
4870  联通|湖南长沙　　　　↑ 645.94    ↓ 690.67    128.71  
25858 移动|北京　　　　　　↑ 158.37    ↓ 2971.44   259.69  
16398 移动|贵州贵阳　　　　↑ 547.85    ↓ 4847.93   131.31  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 5 分 35 秒
  当前时间: 2022-03-25 07:23:22
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```




## 伦敦 46.101.85.82

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1999.995 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (135.6 MB Used)
 System uptime      : 0 days, 0 hour 1 min
 Load average       : 0.21, 0.16, 0.07
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : bbr
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : London / GB
 Region             : England
----------------------------------------------------------------------
 I/O Speed(1st run) : 935 MB/s
 I/O Speed(2nd run) : 1.2 GB/s
 I/O Speed(3rd run) : 1.2 GB/s
 I/O Speed(average) : 1130.9 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1998.07 Mbps      4940.20 Mbps        1.23 ms
```


```bash
###############################################################
#  流解锁测试 StreamUnlockTest
#  当前版本: v1.2.2
#  开源地址: https://github.com/LovelyHaochi/StreamUnlockTest
###############################################################
#  国家代码对照表: http://www.loglogo.com/front/countryCode/
#  测试时间: Fri Mar 25 07:15:53 UTC 2022
###############################################################
正在更新软件包列表...
正在安装依赖: jq

- IPV4 -
 IP:                                    46.101.85.82
 Country:                               United Kingdom
 Region:                                England
 City:                                  London
 ISP:                                   DigitalOcean
 Org:                                   Digitalocean

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               No
 HBO Max:                               No
 Paramount+:                            Yes
 Peacock TV:                            No
 Sling TV:                              No
 Pluto TV:                              Yes
 encoreTVB:                             No
 ABC:                                   No

 -- Europe --
 BritBox:                               Yes
 ITV Hub:                               Yes
 Channel 4:                             Yes
 BBC iPLAYER:                           Yes
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: GB)
 Amazon Prime Video:                    Yes(Region: GB)
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: GB)
 Viu.com:                               No
 Steam:                                 Yes(Currency: GBP)

```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3973  电信|甘肃兰州　　　　↑ 3.20      ↓ 4.60      250.95  
24447 联通|上海５Ｇ　　　　↑ 213.49    ↓ 340.39    342.46  
27154 联通|天津５Ｇ　　　　↑ 224.04    ↓ 420.56    303.41  
13704 联通|江苏南京　　　　↑ 233.92    ↓ 55.78     286.01  
4870  联通|湖南长沙　　　　↑ 237.09    ↓ 278.94    247.37  
25858 移动|北京　　　　　　↑ 210.78    ↓ 2985.56   199.49  
16398 移动|贵州贵阳　　　　↑ 271.33    ↓ 2732.12   293.00  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 5 分 11 秒
  当前时间: 2022-03-25 07:51:36
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```



## 法兰克福 206.189.48.191

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1996.250 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (135.9 MB Used)
 System uptime      : 0 days, 0 hour 2 min
 Load average       : 0.13, 0.15, 0.06
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : bbr
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : Frankfurt am Main / DE
 Region             : Hesse
----------------------------------------------------------------------
 I/O Speed(1st run) : 843 MB/s
 I/O Speed(2nd run) : 1.0 GB/s
 I/O Speed(3rd run) : 1.1 GB/s
 I/O Speed(average) : 997.8 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1997.57 Mbps      14435.15 Mbps       0.24 m
```

```bash
###############################################################
#  流解锁测试 StreamUnlockTest
#  当前版本: v1.2.2
#  开源地址: https://github.com/LovelyHaochi/StreamUnlockTest
###############################################################
#  国家代码对照表: http://www.loglogo.com/front/countryCode/
#  测试时间: Fri Mar 25 07:33:54 UTC 2022
###############################################################
正在更新软件包列表...
正在安装依赖: jq

- IPV4 -
 IP:                                    206.189.48.191
 Country:                               Germany
 Region:                                Hesse
 City:                                  Frankfurt am Main
 ISP:                                   DigitalOcean, LLC
 Org:                                   Digital Ocean

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               No
 HBO Max:                               No
 Paramount+:                            Yes
 Peacock TV:                            No
 Sling TV:                              No
 Pluto TV:                              Yes
 encoreTVB:                             No
 ABC:                                   No

 -- Europe --
 BritBox:                               No
 ITV Hub:                               No
 Channel 4:                             No
 BBC iPLAYER:                           No
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: DE)
 Amazon Prime Video:                    Yes(Region: DE)
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: DE)
 Viu.com:                               No
 Steam:                                 Yes(Currency: EUR)

```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 85.37     ↓ 3038.24   237.09  
17145 电信|安徽合肥５Ｇ　　↑ 115.98    ↓ 2561.60   235.96  
27594 电信|广东广州５Ｇ　　↑ 0.60      ↓ 110.51    247.76  
5396  电信|江苏苏州５Ｇ　　↑ 308.88    ↓ 2321.77   251.37  
23844 电信|湖北武汉　　　　↑ 8.59      ↓ 1435.58   270.93  
29353 电信|湖北武汉５Ｇ　　↑ 4.64      ↓ 32.84     280.42  
28225 电信|湖南长沙５Ｇ　　↑ 105.95    ↓ 2.77      360.18
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 5 分 11 秒
  当前时间: 2022-03-25 07:51:36
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```


## 多伦多 138.197.147.167


```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1999.997 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (136.1 MB Used)
 System uptime      : 0 days, 0 hour 2 min
 Load average       : 0.26, 0.25, 0.10
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : bbr
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : Toronto / CA
 Region             : Ontario
----------------------------------------------------------------------
 I/O Speed(1st run) : 789 MB/s
 I/O Speed(2nd run) : 914 MB/s
 I/O Speed(3rd run) : 888 MB/s
 I/O Speed(average) : 863.7 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1999.06 Mbps      7286.04 Mbps        0.48 ms
```


```bash
###############################################################
#  流解锁测试 StreamUnlockTest
#  当前版本: v1.2.2
#  开源地址: https://github.com/LovelyHaochi/StreamUnlockTest
###############################################################
#  国家代码对照表: http://www.loglogo.com/front/countryCode/
#  测试时间: Fri Mar 25 07:33:56 UTC 2022
###############################################################
正在更新软件包列表...
正在安装依赖: jq

- IPV4 -
 IP:                                    138.197.147.167
 Country:                               Canada
 Region:                                Ontario
 City:                                  Toronto
 ISP:                                   DigitalOcean, LLC
 Org:                                   Digital Ocean

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               No
 HBO Max:                               No
 Paramount+:                            Yes
 Peacock TV:                            No
 Sling TV:                              Yes
 Pluto TV:                              Yes
 encoreTVB:                             No
 ABC:                                   No

 -- Europe --
 BritBox:                               Yes
 ITV Hub:                               No
 Channel 4:                             No
 BBC iPLAYER:                           No
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: CA)
 Amazon Prime Video:                    Yes(Region: CA)
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: CA)
 Viu.com:                               No
 Steam:                                 Yes(Currency: CAD)

```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 44.88     ↓ 3449.03   229.40  
17145 电信|安徽合肥５Ｇ　　↑ 86.20     ↓ 1033.86   222.60  
27594 电信|广东广州５Ｇ　　↑ 238.10    ↓ 926.62    233.41  
5396  电信|江苏苏州５Ｇ　　↑ 376.70    ↓ 2630.26   208.98  
23844 电信|湖北武汉　　　　↑ 11.16     ↓ 107.61    231.62  
29353 电信|湖北武汉５Ｇ　　↑ 21.79     ↓ 83.98     252.64  
28225 电信|湖南长沙５Ｇ　　↑ 11.47     ↓ 889.56    241.69  
3973  电信|甘肃兰州　　　　↑ 3.38      ↓ 18.18     260.17  
24447 联通|上海５Ｇ　　　　↑ 353.05    ↓ 511.70    246.40  
27154 联通|天津５Ｇ　　　　↑ 184.61    ↓ 90.69     278.23  
13704 联通|江苏南京　　　　↑ 172.61    ↓ 24.46     293.51  
4870  联通|湖南长沙　　　　↑ 156.52    ↓ 20.39     253.53  
25858 移动|北京　　　　　　↑ 323.61    ↓ 1545.22   249.11  
16398 移动|贵州贵阳　　　　↑ 303.27    ↓ 1488.98   248.70  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 8 分 3 秒
  当前时间: 2022-03-25 07:44:24
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```

## 班加罗尔 64.227.171.221


```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2022-02-22
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : DO-Premium-AMD
 CPU Cores          : 1 @ 1999.999 MHz
 CPU Cache          : 512 KB
 AES-NI             : Enabled
 VM-x/AMD-V         : Enabled
 Total Disk         : 24.2 GB (1.5 GB Used)
 Total Mem          : 976.9 MB (135.9 MB Used)
 System uptime      : 0 days, 0 hour 1 min
 Load average       : 0.28, 0.14, 0.05
 OS                 : Ubuntu 20.04.3 LTS
 Arch               : x86_64 (64 Bit)
 Kernel             : 5.4.0-97-generic
 TCP CC             : bbr
 Virtualization     : KVM
 Organization       : AS14061 DigitalOcean, LLC
 Location           : Doddaballapura / IN
 Region             : Karnataka
----------------------------------------------------------------------
 I/O Speed(1st run) : 640 MB/s
 I/O Speed(2nd run) : 1.1 GB/s
 I/O Speed(3rd run) : 1.1 GB/s
 I/O Speed(average) : 964.3 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency     
 Speedtest.net    1951.26 Mbps      27.32 Mbps          1.12 ms
```


```bash
###############################################################
#  流解锁测试 StreamUnlockTest
#  当前版本: v1.2.2
#  开源地址: https://github.com/LovelyHaochi/StreamUnlockTest
###############################################################
#  国家代码对照表: http://www.loglogo.com/front/countryCode/
#  测试时间: Fri Mar 25 07:34:12 UTC 2022
###############################################################
正在更新软件包列表...
正在安装依赖: jq

- IPV4 -
 IP:                                    64.227.171.221
 Country:                               India
 Region:                                Karnataka
 City:                                  Bengaluru
 ISP:                                   DigitalOcean, LLC
 Org:                                   DigitalOcean, LLC

 -- Hong Kong --
 MyTVSuper:                             No
 Now E:                                 No
 ViuTV:                                 No
 BiliBili Hongkong/Macau/Taiwan:        No

 -- Taiwan --
 4GTV.TV:                               No
 KKTV:                                  No
 Hami Video:                            No
 LineTV.TW:                             No
 Bahamut Anime:                         No
 Bilibili Taiwan Only:                  No

 -- Japan --
 Abema.TV:                              No
 Niconico:                              Yes
 Paravi:                                No
 U-NEXT:                                No
 Hulu Japan:                            No
 Fuji TV:                               No
 Radiko:                                No
 DMM:                                   Yes
 Princess Connect Re:Dive Japan:        No
 Pretty Derby Japan:                    No
 Kancolle Japan:                        No
 ErogameScape:                          Yes

 -- Korea --
 Tving:                                 No
 KakaoTV:                               Yes

 -- United States --
 Hulu United States:                    ->/dev/fd/63: line 701: warning: command substitution: ignored null byte in input
parse error: Invalid numeric literal at line 1, column 48
 Hulu United States:                    Yes
 HBO Now:                               No
 HBO Max:                               No
 Paramount+:                            No
 Peacock TV:                            No
 Sling TV:                              No
 Pluto TV:                              No
 encoreTVB:                             No
 ABC:                                   No

 -- Europe --
 BritBox:                               No
 ITV Hub:                               No
 Channel 4:                             No
 BBC iPLAYER:                           No
 Molotov:                               No

 -- Porn --
 Biguz:                                 No
 Blacked:                               Yes

 -- Global --
 DAZN:                                  No
 Netflix:                               Only Homemade
 DisneyPlus:                            No
 YouTube:                               Yes(Region: IN)
 Amazon Prime Video:                    No
 Tiktok:                                Failed
 iQiyi Global:                          Yes(Region: IN)
 Viu.com:                               No
 Steam:                                 Yes(Currency: INR)

```

```bash
———————————————————SuperSpeed 全面测速版——————————————————
       bash <(curl -Lso- https://raw.githubusercontent.com/BlueSkyXN/SpeedTestCN/main/superspeed.sh)
       如果仍然异常，应该是SpeedTest初次授权问题
       请使用工具箱安装SpeedTest然后手动运行后YES授权
——————————————————————————————————————————————————————————
  测速类型:    1. 三网测速    2. 取消测速
               3. 电信节点    4. 联通节点    5. 移动节点
  请输入数字选择测速类型: 1
——————————————————————————————————————————————————————————
ID    测速服务器信息       上传/Mbps   下载/Mbps   延迟/ms
3633  电信|上海　　　　　　↑ 40.17     ↓ 1082.75   369.76  
17145 电信|安徽合肥５Ｇ　　↑ 28.27     ↓ 791.64    368.51  
27594 电信|广东广州５Ｇ　　↑ 17.79     ↓ 27.76     399.52  
5396  电信|江苏苏州５Ｇ　　↑ 208.06    ↓ 1312.64   355.98  
23844 电信|湖北武汉　　　　↑ 13.24     ↓ 52.26     380.43  
29353 电信|湖北武汉５Ｇ　　↑ 1.13      ↓ 24.68     372.02  
28225 电信|湖南长沙５Ｇ　　↑ 191.29    ↓ 242.79    420.77  
3973  电信|甘肃兰州　　　　↑ 40.06     ↓ 5.06      413.55  
24447 联通|上海５Ｇ　　　　↑ 381.38    ↓ 3887.87   204.34  
27154 联通|天津５Ｇ　　　　↑ 386.32    ↓ 3651.52   210.02  
13704 联通|江苏南京　　　　↑ 369.68    ↓ 952.54    225.59  
4870  联通|湖南长沙　　　　↑ 203.21    ↓ 976.14    188.89  
25858 移动|北京　　　　　　↑ 265.69    ↓ 2643.37   282.61  
16398 移动|贵州贵阳　　　　↑ 294.86    ↓ 2235.91   264.63  
——————————————————————————————————————————————————————————
  测试完成, 本次测速耗时: 8 分 21 秒
  当前时间: 2022-03-25 07:44:44
  # 三网测速中为避免节点数不均及测试过久，每部分未使用所
  # 有节点，如果需要使用全部节点，可分别选择三网节点检测
```
