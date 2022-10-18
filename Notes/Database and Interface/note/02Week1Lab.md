# Week1 Lab

VSCode

Chrome

## Networking Commands

### ping

```bash
ping <host>
```

sends a series of packets and expects to receive a response to each packet.

**exercise**

www.bilibili.com

```bash
C:\WINDOWS\system32>ping www.bilibili.com

Pinging a.w.bilicdn1.com [61.240.206.10] with 32 bytes of data:
Reply from 61.240.206.10: bytes=32 time=39ms TTL=49
Reply from 61.240.206.10: bytes=32 time=41ms TTL=49
Reply from 61.240.206.10: bytes=32 time=70ms TTL=49
Reply from 61.240.206.10: bytes=32 time=40ms TTL=49

Ping statistics for 61.240.206.10:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 39ms, Maximum = 70ms, Average = 47ms
```

www.google.com

```bash
C:\WINDOWS\system32>ping www.google.com

Pinging www.google.com [142.250.204.36] with 32 bytes of data:
Reply from 142.250.204.36: bytes=32 time=47ms TTL=119
Reply from 142.250.204.36: bytes=32 time=97ms TTL=119
Reply from 142.250.204.36: bytes=32 time=43ms TTL=119
Reply from 142.250.204.36: bytes=32 time=36ms TTL=119

Ping statistics for 142.250.204.36:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 36ms, Maximum = 97ms, Average = 55ms
```

www.nottingham.edu.cn

```bash
C:\WINDOWS\system32>ping nottingham.edu.cn

Pinging nottingham.edu.cn [10.2.1.3] with 32 bytes of data:
Reply from 10.2.1.3: bytes=32 time=3ms TTL=125
Reply from 10.2.1.3: bytes=32 time=2ms TTL=125
Reply from 10.2.1.3: bytes=32 time=5ms TTL=125
Reply from 10.2.1.3: bytes=32 time=4ms TTL=125

Ping statistics for 10.2.1.3:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 2ms, Maximum = 5ms, Average = 3ms
```

### nslookup

```bash
nslookup <host>
```

performs "nameserver lookup" using DNS server

identify IP address for a domain name

**exercise**

www.bilibili.com

```bash
C:\WINDOWS\system32>nslookup www.bilibili.com
Server:  DC02.nottingham.edu.cn
Address:  10.2.1.6

Non-authoritative answer:
Name:    a.w.bilicdn1.com
Addresses:  2408:8752:e00:600::2
          2408:873c:5810:3:0:1:0:4
          2408:8752:e00:600::3
          2408:8752:e00:600::4
          2408:8752:e00:600::5
          2408:873c:5810:3:0:1:0:2
          2408:873c:5810:3:0:1:0:3
          2408:873c:5810:3:0:1:0:5
          58.241.133.58
          61.240.206.10
          61.240.206.11
          61.240.206.13
          61.240.206.12
          58.241.133.34
          58.241.133.50
          58.241.133.52
          58.241.133.54
          58.241.133.56
Aliases:  www.bilibili.com
```

www.google.com

```bash
C:\WINDOWS\system32>nslookup www.google.com
Server:  DC02.nottingham.edu.cn
Address:  10.2.1.6

Non-authoritative answer:
Name:    www.google.com
Addresses:  2404:6800:4005:812::2004
          142.250.204.36
```

www.nottingham.edu.cn

```bash
C:\WINDOWS\system32>nslookup www.nottingham.edu.cn
Server:  DC02.nottingham.edu.cn
Address:  10.2.1.6

Name:    live-china-uon.asia.contensis.com
Addresses:  2400:3200:1600::275
          118.178.243.203
Aliases:  www.nottingham.edu.cn
```

### Traceroute

```bash
tracert <host>
```

show the routers that a package encounters on their way to the <host>

**exercise**

```bash
C:\WINDOWS\system32>tracert nottingham.ac.uk

Tracing route to nottingham.ac.uk [185.18.139.133]
over a maximum of 30 hops:

  1    79 ms     3 ms     4 ms  10.176.0.2
  2    10 ms     5 ms     5 ms  10.253.0.4
  3     *        *        *     Request timed out.
  4     8 ms     *       13 ms  61.175.6.89
  5     7 ms     5 ms     7 ms  59.43.65.17
  6    59 ms     7 ms     8 ms  59.43.117.165
  7     9 ms    16 ms    15 ms  59.43.47.93
  8     *        *        *     Request timed out.
  9    22 ms    14 ms    67 ms  59.43.246.190
 10   275 ms   211 ms   213 ms  59.43.250.22
 11     *      292 ms   275 ms  9-1-7.ear1.london15.level3.net [217.163.47.129]
 12   231 ms   210 ms   209 ms  ae1.3110.edge3.london1.level3.net [4.69.140.198]
 13   222 ms   213 ms   350 ms  unknown.level3.net [212.113.11.36]
 14   213 ms   226 ms   212 ms  185.18.139.133

Trace complete.
```

### whois

> This command cannot use in Windows

give detailed info about domain names and IP address

