# A200002_STP
Proyecto STP - Conmutadores y Redes Inalambricas
SWITCH1
SW1>enable
SW1#configure terminal
SW1(config)#hostname Switch1
Switch1(config)#enable secret cisco
Switch1(config)#no ip domain lookup
Switch1(config)#interface Vlan1
Switch1(config-if)#ip address 192.168.1.1 255.255.255.0
Switch1(config-if)#no shut
Switch1(config-if)#line con 0
Switch1(config-line)#exec-timeout 0 0
Switch1(config-line)#logging synchronous
Switch1(config-line)#password cisco2
Switch1(config-line)#login
Switch1(config-line)#exit
Switch1(config)#line vty 0 15
Switch1(config-line)#logging synchronous
Switch1(config-line)#password cisco3
Switch1(config-line)#login
Switch1(config-line)#end
Switch1#copy running-config startup-config

Switch1(config)#interface range fastEthernet 1/1 - 3
Switch1(config-if-range)#switchport mode trunk
Switch1(config-if-range)#no shutdown 
Switch1(config-if-range)#end
Switch1#

=============================================

SWITCH2
SW2>enable
SW2#configure terminal
SW2(config)#hostname Switch2
Switch2(config)#enable secret cisco
Switch2(config)#no ip domain lookup
Switch2(config)#interface Vlan1
Switch2(config-if)#ip address 192.168.1.2 255.255.255.0
Switch2(config-if)#no shut
Switch2(config-if)#line con 0
Switch2(config-line)#exec-timeout 0 0
Switch2(config-line)#logging synchronous
Switch2(config-line)#password cisco2
Switch2(config-line)#login
Switch2(config-line)#exit
Switch2(config)#line vty 0 15
Switch2(config-line)#logging synchronous
Switch2(config-line)#password cisco3
Switch2(config-line)#login
Switch2(config-line)#end
Switch2#copy running-config startup-config

Switch2(config)#interface range fastEthernet 1/1 - 3
Switch2(config-if-range)#switchport mode trunk
Switch2(config-if-range)#no shutdown 
Switch2(config-if-range)#end
Switch2#

============================================

SWITCH3
SW3>enable
SW3#configure terminal
SW3(config)#hostname Switch3
Switch3(config)#enable secret cisco
Switch3(config)#no ip domain lookup
Switch3(config)#interface Vlan1
Switch3(config-if)#ip address 192.168.1.3 255.255.255.0
Switch3(config-if)#no shut
Switch3(config-if)#line con 0
Switch3(config-line)#exec-timeout 0 0
Switch3(config-line)#logging synchronous
Switch3(config-line)#password cisco2
Switch3(config-line)#login
Switch3(config-line)#exit
Switch3(config)#line vty 0 15
Switch3(config-line)#logging synchronous
Switch3(config-line)#password cisco3
Switch3(config-line)#login
Switch3(config-line)#end
Switch3#copy running-config startup-config

Switch3(config)#interface range fastEthernet 1/1 - 3
Switch3(config-if-range)#switchport mode trunk
Switch3(config-if-range)#no shutdown 
Switch3(config-if-range)#end
Switch3#

=========================================

SWITCH4
SW4>enable
SW4#configure terminal
SW4(config)#hostname Switch4
Switch4(config)#enable secret cisco
Switch4(config)#no ip domain lookup
Switch4(config)#interface Vlan1
Switch4(config-if)#ip address 192.168.1.4 255.255.255.0
Switch4(config-if)#no shut
Switch4(config-if)#line con 0
Switch4(config-line)#exec-timeout 0 0
Switch4(config-line)#logging synchronous
Switch4(config-line)#password cisco2
Switch4(config-line)#login
Switch4(config-line)#exit
Switch4(config)#line vty 0 15
Switch4(config-line)#logging synchronous
Switch4(config-line)#password cisco3
Switch4(config-line)#login
Switch4(config-line)#end
Switch4#copy running-config startup-config


Switch4(config)#interface range fastEthernet 1/1 - 3
Switch4(config-if-range)#switchport mode trunk
Switch4(config-if-range)#no shutdown 
Switch4(config-if-range)#end
Switch4#

=================================================
