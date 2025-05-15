# Cisco Router & Switch Configuration Commands (Putty Console)

## Basic Privileged Access
enable
configure terminal



## Set Hostname (Based on Router)
hostname mia // or nyc, san, chi



## Encrypt Enable Mode Password
enable secret mia // or nyc, chi, san



## Set Console Line Password
line console 0
password mia // or nyc, chi, san
login


## Encrypt All Plain Text Passwords
service password-encryption


## Deterrent Control (Banner Message)
banner motd "unauthorized login attempts are prohibited"


## Disable DNS Lookup (Avoid Delay on Mistyped Commands)
no ip domain-lookup



## Assign IP Address to Interface
interface GigabitEthernet0/1 or G0/2
ip address 172.30.32.2 255.255.255.255
no shutdown
exit


## Set Default Gateway (on Switches)
ip default-gateway 172.30.32.1


## Shutdown an Unused Port
interface GigabitEthernet0/0
shutdown
exit


## Telnet Configuration
line vty 0 15
password yourpassword
login
transport input telnet


## SSH Configuration
ip domain-name anydomain.com
crypto key generate rsa
// When prompted, enter key size: 1024 or 2048
username project password project123
line vty 0 15
login local
transport input ssh


## SSH Access Example
ssh project@172.30.0.1


## Enable OSPF (Dynamic Routing)
router ospf 1
network 172.30.0.0 0.0.255.255 area 0




### Show IP Routes
show ip route



### Show Running Configuration
show running-config



### Show MAC Address Table (for Switches)
show mac-address-table
