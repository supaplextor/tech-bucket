<pre><code>supaplex@sky:~/usr/src/github-by-user/supaplextor/aqemu$ sudo brctl show
bridge name     bridge id               STP enabled     interfaces
br0             8000.261cda934529       no              eno1
br1             8000.5250e06fd466       no              tap0
                                                        tap1
supaplex@sky:~/usr/src/github-by-user/supaplextor/aqemu$ ip l
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN mode DEFAULT group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
2: eno1: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel master br0 state UP mode DEFAULT group default qlen 1000
    link/ether a0:ad:9f:32:ab:f8 brd ff:ff:ff:ff:ff:ff
    altname enp9s0
    altname enxa0ad9f32abf8
3: br0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue state UP mode DEFAULT group default qlen 1000
    link/ether 26:1c:da:93:45:29 brd ff:ff:ff:ff:ff:ff
4: wlp10s0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue state DOWN mode DORMANT group default qlen 1000
    link/ether 92:79:ee:e7:52:e4 brd ff:ff:ff:ff:ff:ff permaddr 58:02:05:6d:69:70
    altname wlx5802056d6970
6: br1: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN mode DEFAULT group default qlen 1000
    link/ether 52:50:e0:6f:d4:66 brd ff:ff:ff:ff:ff:ff
7: tap0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel master br1 state UNKNOWN mode DEFAULT group default qlen 1000
    link/ether fe:5e:81:bc:25:8a brd ff:ff:ff:ff:ff:ff
8: tap1: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel master br1 state UNKNOWN mode DEFAULT group default qlen 1000
    link/ether fe:f5:8a:04:6c:82 brd ff:ff:ff:ff:ff:ff
</code></pre>
