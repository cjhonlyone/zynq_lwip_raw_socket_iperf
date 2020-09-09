# -----lwIP Socket Mode Demo Application ------
Board IP: 192.168.1.10
Netmask : 255.255.255.0
Gateway : 192.168.1.1
Start PHY autonegotiation 
Waiting for PHY to complete autonegotiation.
autonegotiation complete 
link speed for phy address 0: 1000

              Server   Port Connect With..
-------------------- ------ --------------------
       rxperf server   5001 $ iperf -c <board ip> -i 5 -t 50 -w 64k
       txperf client    N/A $ iperf -s -i 5 -t 100 (on host with IP 192.168.1.100)
Rx performance : 450Mbps

Tx performance : 600Mbps

# -----lwIP RAW Mode Demo Application ------
Start PHY autonegotiation 
Waiting for PHY to complete autonegotiation.
autonegotiation complete 
link speed for phy address 0: 1000
DHCP Timeout
Configuring default IP of 192.168.1.10
Board IP:       192.168.1.10
Netmask :       255.255.255.0
Gateway :       192.168.1.1

              Server   Port Connect With..
-------------------- ------ --------------------
       rxperf server   5001 $ iperf -c <board ip> -i 5 -t 100
       txperf client    N/A $ iperf -s -i 5 -w 64k (on host with IP 192.168.1.100)
Rx performance : 950Mbps

Tx performance : 950Mbps