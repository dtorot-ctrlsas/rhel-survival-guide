# rhel-survival-guide
RH survival guide notes

## Networking
+ interfaces
  - ethernet: en
  - wlan: wl
  - wwan: ww
  - on-board: o#
  - pci hotplug slot: s#
  - bus/slot PCI: p#s#
  - card multi función: f#
  - enp0s1f0: función 0, eth card, bus 0, slot 1
+ network address
  - host 172.168.181.23
    - 10101100.10101000.10110101.00010111
  - Network prefix /19 255.255.224.0
    - 11111111.11111111.11100000.00000000
  - Network addr 172.168.160.0
    - 10101100.10101000.10100000.00000000
  - Broadcast addr 172.168.191.255
    - 10101100.10101000.10111111.11111111
+ ipv6
  - suppress leading zeros
  - shorten :: the repeated zeros groups and :0: in zero group, with :: in leftmost and :0: in rightmost
  - use port with brackets > [ipv6]:port  
  - ipv6 address {IMAGE}
  - multicast ipv6 address: ff02::1
  - default route in a ipv6 net> ::/0 
  - with identifier: ff02::1%ens3 use with ping6…
  - discovery of ipv6 hosts in the network: ip -6 route
  - traceroute -6 
  - tracepath6

### Commands
+ `ip link show`
+ `ip addr show ens3`
+ `ip -s link show ens3`
+ `tracepath google.com`
  - _MTU_: max transmission unit size
  - _RTT_: round trip timing
  - _asymm_: traffic from that router returned from other route

