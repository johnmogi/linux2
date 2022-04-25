ping between computer an vm

windows: ipconfig // 192.168.10.105 
linux - ifconfig (old) // 
route -n

ping 192.168.10.0
ping 192.168.1.89
192.168.10.105 

delete network-
ifconfig eth0 0.0.0.0. netmask 0.0.0.0
ok - all deleted - now add with route / ip ...
ifconfig eth0 192.168.1.0 netmask 255.255.255.0
192.168.10.0 
route -n // old method
ip route show // shows ip with netmask "/24" = 255.255.255.0


192.168.1.0

add default gateway:
route add default gw 192.168.1.1 eth0 // old method
ip route add default via 192.168.1.1
restart service:
(reconnect cable manually to vm box)



