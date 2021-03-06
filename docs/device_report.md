# Device 9a:02:57:1e:8f:01, *** Make *** *** Model ***

## Test Roles

|  Role  |      Name              | Status |
|--------|------------------------|--------|
|Operator| *** Operator Name *** |        |
|Approver| *** Approver Name *** |        |

## Test Iteration

| Test parameter   | Value                  |
|------------------|------------------------|
| Test report start date | XXX |
| Test report end date   | XXX |
|
| Attempt number   | 1 |

## Device Identification

| Device            | Entry              |
|-------------------|--------------------|
| Name              | *** Name *** |
| GUID              | *** GUID *** |
| MAC addr          | 9a:02:57:1e:8f:01 |
| Hostname          | *** Network Hostname *** |
| Type              | *** Type *** |
| Make              | *** Make *** |
| Model             | *** Model *** |
| Serial Number     | *** Serial *** |
| Firmware Version  | *** Firmware Version *** |

## Device Description

![Image of device](*** Device Image URL ***)

*** Device Description ***


### Device documentation

[Device datasheets](*** Device Datasheets URL ***)
[Device manuals](*** Device Manuals URL ***)

## Report summary

Overall device result FAIL

**Some tests report as GONE. Please check for possible misconfiguration**

|Category|Total Tests|Result|Required Pass|Required Pass for PoE Devices|Required Pass for BACnet Devices|Recommended Pass|Information|Other|
|---|---|---|---|---|---|---|---|---|
|Connection|9|FAIL|1/4/4|0/0/0|0/0/0|0/0/0|0/0/0|0/0/0|
|Security|8|FAIL|1/0/4|0/0/0|0/0/0|1/1/0|0/0/1|0/0/0|
|Network Time|2|PASS|2/0/0|0/0/0|0/0/0|0/0/0|0/0/0|0/0/0|
|TLS|0|N/A|0/0/0|0/0/0|0/0/0|0/0/0|0/0/0|0/0/0|
|Protocol|2|FAIL|0/0/0|0/0/0|0/1/0|0/0/0|0/0/1|0/0/0|
|PoE|3|FAIL|0/0/0|0/1/1|0/0/0|0/0/0|0/1/0|0/0/0|
|BOS|1|SKIP|0/0/0|0/0/0|0/0/0|0/0/1|0/0/0|0/0/0|
|Other|2|GONE|0/0/0|0/0/0|0/0/0|0/0/0|0/0/0|0/2/0|
|Communication|2|GONE|0/1/0|0/0/0|0/0/0|0/0/0|0/1/0|0/0/0|
Syntax: Pass / Fail / Skip

|Expectation|pass|fail|skip|info|gone|
|---|---|---|---|---|---|
|Required Pass|4|1|8|0|4|
|Required Pass for PoE Devices|0|0|1|0|1|
|Required Pass for BACnet Devices|0|1|0|0|0|
|Recommended Pass|1|0|1|0|1|
|Information|0|0|2|0|2|
|Other|3|0|10|2|2|

|Result|Test|Category|Expectation|Notes|
|---|---|---|---|---|
|pass|base.startup.dhcp|Other|Other||
|skip|base.switch.ping|Connection|Required Pass|No local IP has been set, check system config|
|skip|cloud.udmi.event_pointset|BOS|Recommended Pass|No device id|
|skip|cloud.udmi.event_system|Other|Other|No device id|
|skip|cloud.udmi.provision|Other|Other|No device id|
|skip|cloud.udmi.state_pointset|Other|Other|No device id|
|skip|cloud.udmi.state_system|Other|Other|No device id|
|pass|communication.network.min_send|Other|Other|ARP packets received. Data packets were sent at a frequency of less than 5 minutes|
|info|communication.network.type|Other|Other|Broadcast packets received. Unicast packets received.|
|pass|connection.base.target_ping|Connection|Required Pass|target reached|
|gone|connection.ipaddr.dhcp_disconnect|Connection|Required Pass||
|gone|connection.ipaddr.private_address|Connection|Required Pass||
|gone|connection.network.communication_min_send|Communication|Required Pass||
|gone|connection.network.communication_type|Communication|Information||
|gone|connection.network.dhcp_long|Connection|Required Pass||
|info|connection.network.mac_address|Other|Other|Device MAC address is 9a:02:57:1e:8f:01|
|fail|connection.network.mac_oui|Connection|Required Pass|Manufacturer prefix not found!|
|skip|connection.switch.port_duplex|Connection|Required Pass|No local IP has been set, check system config|
|skip|connection.switch.port_link|Connection|Required Pass|No local IP has been set, check system config|
|skip|connection.switch.port_speed|Connection|Required Pass|No local IP has been set, check system config|
|skip|dns.network.hostname_resolution|Other|Other|Device did not send any DNS requests|
|pass|manual.test.name|Security|Recommended Pass|Manual test - for testing|
|pass|ntp.network.ntp_support|Network Time|Required Pass|Using NTPv4.|
|pass|ntp.network.ntp_update|Network Time|Required Pass|Device clock synchronized.|
|gone|poe.switch.negotiation|PoE|Required Pass for PoE Devices||
|skip|poe.switch.power|PoE|Required Pass for PoE Devices|No local IP has been set, check system config|
|gone|poe.switch.support|PoE|Information||
|fail|protocol.bacext.pic|Protocol|Required Pass for BACnet Devices|PICS file defined however a BACnet device was not found.|
|skip|protocol.bacext.version|Protocol|Information|Bacnet device not found.|
|skip|security.discover.firmware|Security|Information|Could not retrieve a firmware version with nmap. Check bacnet port.|
|pass|security.nmap.http|Other|Other|No running http servers have been found.|
|pass|security.nmap.ports|Security|Required Pass|Only allowed ports found open.|
|skip|security.password.http|Security|Required Pass|Port 80 not open on target device.|
|skip|security.password.https|Security|Required Pass|Port 443 not open on target device.|
|skip|security.password.ssh|Security|Required Pass|Port 22 not open on target device.|
|skip|security.password.telnet|Security|Required Pass|Port 23 not open on target device.|
|gone|security.ports.nmap|Security|Recommended Pass||
|skip|security.tls.v1_2_client|Other|Other|No client initiated TLS communication detected|
|skip|security.tls.v1_2_server|Other|Other|IOException unable to connect to server.|
|skip|security.tls.v1_3_client|Other|Other|No client initiated TLS communication detected|
|skip|security.tls.v1_3_server|Other|Other|IOException unable to connect to server.|
|skip|security.tls.v1_server|Other|Other|IOException unable to connect to server.|
|gone|unknown.fake.llama|Other|Other||
|gone|unknown.fake.monkey|Other|Other||


## Module pass


#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|

## Module ping


#### Report

```
--------------------
Baseline ping test report

LOCAL_IP not configured, assuming no network switch

Done with basic connectivity tests

--------------------
base.startup.dhcp
--------------------
Check the base DHCP startup exchange
--------------------
See log above
--------------------
RESULT pass base.startup.dhcp

--------------------
base.switch.ping
--------------------
Attempt to ping access switch (if configured)
--------------------
See log above
--------------------
RESULT skip base.switch.ping No local IP has been set, check system config

--------------------
connection.base.target_ping
--------------------
Attempt to ping the Device Under Test
--------------------
See log above
--------------------
RESULT pass connection.base.target_ping target reached

```

## Module nmap


#### Report

```
--------------------
security.nmap.ports
--------------------
Automatic TCP/UDP port scan using nmap
--------------------
# Nmap XXX scan initiated XXX as: nmap -v -n -T5 -sT -sU --host-timeout=4m --open -pU:47808,T:23,443,80, -oG XXX/tmp/nmap.log X.X.X.X
# Ports scanned: TCP(3;23,80,443) UDP(1;47808) SCTP(0;) PROTOCOLS(0;)
Host: X.X.X.X () Status: Up
Host: X.X.X.X () Ports: 47808/closed/udp//bacnet///
# Nmap done at XXX -- 1 IP address (1 host up) scanned in XXX
No invalid ports found.
--------------------
RESULT pass security.nmap.ports Only allowed ports found open.

--------------------
security.nmap.http
--------------------
Check that the device does not have open ports exposing an unencrypted web interface using HTTP
--------------------
# Nmap XXX scan initiated XXX as: nmap -v -n -T5 -A --script http-methods --host-timeout=4m --open -p- -oG XXX/tmp/http.log X.X.X.X
# Ports scanned: TCP(65535;1-65535) UDP(0;) SCTP(0;) PROTOCOLS(0;)
Host: X.X.X.X () Status: Up
Host: X.X.X.X () Ports: 10000/open/tcp//snet-sensor-mgmt?///
# Nmap done at XXX -- 1 IP address (1 host up) scanned in XXX
No running http servers have been found.
--------------------
RESULT pass security.nmap.http No running http servers have been found.

```

#### Module Config

|Attribute|Value|
|---|---|
|timeout_sec|600|
|enabled|True|

## Module discover


#### Report

```
--------------------
security.discover.firmware
--------------------
Automatic bacnet firmware scan using nmap
--------------------
PORT      STATE  SERVICE
47808/udp closed bacnet
MAC Address: 9A:02:57:1E:8F:01 (Unknown)
--------------------
RESULT skip security.discover.firmware Could not retrieve a firmware version with nmap. Check bacnet port.

```

#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|

## Module switch


#### Report

```
--------------------
connection.switch.port_link
--------------------
Connect the device to the network switch. Check the device and the switch for the green connection light & no errors
--------------------
LOCAL_IP not configured, assuming no network switch.
--------------------
RESULT skip connection.switch.port_link No local IP has been set, check system config

--------------------
connection.switch.port_speed
--------------------
Verify the device auto-negotiates connection speed
--------------------
LOCAL_IP not configured, assuming no network switch.
--------------------
RESULT skip connection.switch.port_speed No local IP has been set, check system config

--------------------
connection.switch.port_duplex
--------------------
Verify the device supports full duplex
--------------------
LOCAL_IP not configured, assuming no network switch.
--------------------
RESULT skip connection.switch.port_duplex No local IP has been set, check system config

--------------------
poe.switch.power
--------------------
Verify that the device draws less than the maximum power allocated by the port. This is 15.4W for 802.3af and 30W for 802.3at
--------------------
LOCAL_IP not configured, assuming no network switch.
--------------------
RESULT skip poe.switch.power No local IP has been set, check system config

```

#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|
|poe|{'enabled': True}|

## Module bacext


#### Report

```
--------------------
protocol.bacext.version
--------------------
Verify and record version of Bacnet used by the device
--------------------
 Bacnet device not found.
--------------------
RESULT skip protocol.bacext.version Bacnet device not found.

--------------------
protocol.bacext.pic
--------------------
Verify BACnet traffic is compliant to the PIC statement
--------------------
PICS file defined however a BACnet device was not found.
--------------------
RESULT fail protocol.bacext.pic PICS file defined however a BACnet device was not found.

```

#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|

## Module tls


#### Report

```
--------------------
Collecting TLS cert from target address

Gathering TLS 1 Server Information....
TLS 1Server Implementation Skipping Test, could not open connection
TLS 1 Server Information Complete.


Gathering TLS 1.2 Server Information....
TLS 1.2Server Implementation Skipping Test, could not open connection
TLS 1.2 Server Information Complete.


Gathering TLS 1.3 Server Information....
TLS 1.3Server Implementation Skipping Test, could not open connection
TLS 1.3 Server Information Complete.


Gathering TLS Client X.X.X.X Information....
TLS Client Information Complete.
Gathering TLS Client X.X.X.X Information....
TLS Client Information Complete.

--------------------
security.tls.v1_2_client
--------------------
Verify the device supports at least TLS 1.2 (as a client)
--------------------
See log above
--------------------
RESULT skip security.tls.v1_2_client No client initiated TLS communication detected

--------------------
security.tls.v1_2_server
--------------------
Verify the device supports TLS 1.2 (as a server)
--------------------
See log above
--------------------
RESULT skip security.tls.v1_2_server IOException unable to connect to server.

--------------------
security.tls.v1_3_client
--------------------
Verify the device supports at least TLS 1.3 (as a client)
--------------------
See log above
--------------------
RESULT skip security.tls.v1_3_client No client initiated TLS communication detected

--------------------
security.tls.v1_3_server
--------------------
Verify the device supports TLS 1.3 (as a server)
--------------------
See log above
--------------------
RESULT skip security.tls.v1_3_server IOException unable to connect to server.

--------------------
security.tls.v1_server
--------------------
Verify the device supports at least TLS 1.0 (as a server)
--------------------
See log above
--------------------
RESULT skip security.tls.v1_server IOException unable to connect to server.

```

#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|
|ca_file|CA_Faux.pem|

## Module password


#### Report

```
--------------------
security.admin.password.http
--------------------
Verify all device manufacturer default passwords are changed for protocol: http, and new passwords are set.
--------------------

Starting Nmap 7.60 ( https://nmap.org ) at XXX
Nmap scan report for daq-faux-1 (X.X.X.X)
Host is up (XXX).

PORT   STATE  SERVICE
80/tcp closed http
MAC Address: 9A:02:57:1E:8F:01 (Unknown)

Nmap done: 1 IP address (1 host up) scanned in XXX
Could not connect to specified port on host.
--------------------
RESULT skip security.password.http Port 80 not open on target device.

--------------------
security.admin.password.https
--------------------
Verify all device manufacturer default passwords are changed for protocol: https, and new passwords are set.
--------------------

Starting Nmap 7.60 ( https://nmap.org ) at XXX
Nmap scan report for daq-faux-1 (X.X.X.X)
Host is up (XXX).

PORT    STATE  SERVICE
443/tcp closed https
MAC Address: 9A:02:57:1E:8F:01 (Unknown)

Nmap done: 1 IP address (1 host up) scanned in XXX
Could not connect to specified port on host.
--------------------
RESULT skip security.password.https Port 443 not open on target device.

--------------------
security.admin.password.ssh
--------------------
Verify all device manufacturer default passwords are changed for protocol: ssh, and new passwords are set.
--------------------

Starting Nmap 7.60 ( https://nmap.org ) at XXX
Nmap scan report for daq-faux-1 (X.X.X.X)
Host is up (XXX).

PORT   STATE  SERVICE
22/tcp closed ssh
MAC Address: 9A:02:57:1E:8F:01 (Unknown)

Nmap done: 1 IP address (1 host up) scanned in XXX
Could not connect to specified port on host.
--------------------
RESULT skip security.password.ssh Port 22 not open on target device.

--------------------
security.admin.password.telnet
--------------------
Verify all device manufacturer default passwords are changed for protocol: telnet, and new passwords are set.
--------------------

Starting Nmap 7.60 ( https://nmap.org ) at XXX
Nmap scan report for daq-faux-1 (X.X.X.X)
Host is up (XXX).

PORT   STATE  SERVICE
23/tcp closed telnet
MAC Address: 9A:02:57:1E:8F:01 (Unknown)

Nmap done: 1 IP address (1 host up) scanned in XXX
Could not connect to specified port on host.
--------------------
RESULT skip security.password.telnet Port 23 not open on target device.

```

#### Module Config

|Attribute|Value|
|---|---|
|dictionary_dir|resources/faux|
|enabled|True|

## Module udmi


#### Report

```
--------------------
cloud.udmi.provision
--------------------
Validates device provision payload.
--------------------
No device id
--------------------
RESULT skip cloud.udmi.provision No device id

--------------------
cloud.udmi.state_system
--------------------
Validates device state_system payload.
--------------------
No device id
--------------------
RESULT skip cloud.udmi.state_system No device id

--------------------
cloud.udmi.state_pointset
--------------------
Validates device state_pointset payload.
--------------------
No device id
--------------------
RESULT skip cloud.udmi.state_pointset No device id

--------------------
cloud.udmi.event_system
--------------------
Validates device event_system payload.
--------------------
No device id
--------------------
RESULT skip cloud.udmi.event_system No device id

--------------------
cloud.udmi.event_pointset
--------------------
Validates device event_pointset payload.
--------------------
No device id
--------------------
RESULT skip cloud.udmi.event_pointset No device id

```

#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|

## Module manual


#### Report

```
--------------------
manual.test.name
--------------------

--------------------
No additional information provided
--------------------
RESULT pass manual.test.name Manual test - for testing

```

#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|

## Module network


#### Report

```
--------------------
communication.network.min_send
--------------------
Device sends data at a frequency of less than 5 minutes.
--------------------











RESULT pass communication.network.min_send ARP packets received. Data packets were sent at a frequency of less than 5 minutes
--------------------
communication.network.type
--------------------
Device sends unicast or broadcast packets.
--------------------


RESULT info communication.network.type Broadcast packets received. Unicast packets received.
--------------------
ntp.network.ntp_support
--------------------
Device supports NTP version 4.
--------------------
RESULT pass ntp.network.ntp_support Using NTPv4.
--------------------
ntp.network.ntp_update
--------------------
Device synchronizes its time to the NTP server.
--------------------
RESULT pass ntp.network.ntp_update Device clock synchronized.
--------------------
connection.network.mac_oui
--------------------
Check Physical device address OUI against IEEE registration and verify it is registered with the correct manufacturer
--------------------
Using the host hardware address 9a:02:57:1e:8f:01
Mac OUI Test
--------------------
RESULT fail connection.network.mac_oui Manufacturer prefix not found!

--------------------
connection.network.mac_address
--------------------
Reports device MAC address
--------------------
Device MAC address is 9a:02:57:1e:8f:01
--------------------
RESULT info connection.network.mac_address Device MAC address is 9a:02:57:1e:8f:01

--------------------
dns.network.hostname_resolution
--------------------
Check device uses the DNS server from DHCP and resolves hostnames
--------------------
RESULT skip dns.network.hostname_resolution Device did not send any DNS requests
```

#### Module Config

|Attribute|Value|
|---|---|
|enabled|True|

## Report complete

