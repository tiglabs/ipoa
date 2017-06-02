# ipoa
IPv4 options Address.

                   +------+-----+-------------+
                   | type | len | real saddr  |
                   +------+----++-------------+
                               ^
                               |
                               |
                               |
    +-------+-----------+------+---------+-------------+----------+
    |l2 hdr |  ipv4 hdr |  ipv4 options  | tcp/udp hdr |   data   |
    +-------+-----------+----------------+-------------+----------+

## what is ipoa?
use IPv4 options to carray the real source address of the NAT-packet. The tcp and udp application can get real client IP address with ipoa.
## which OS we support?
>[root@localhost]cat /etc/redhat-release

>CentOS Linux release 7.2.1511