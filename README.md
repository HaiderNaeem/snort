# snort
Notes and Documentation
Requires additional installation of win pcap 4.1.1 or above
after installation, open commmand line terminal
switch to snort directory, cd \snort
cd bin
snort -V // check for version
etc folder has all configurations
local.rules will have all custom rules

test local.rules:
alert icmp any any -> any any (msg:"Test ICMP Alert"; sid:1000001;)
alert udp any any -> any any (msg:"Test UDP Alert"; sid:1000002;)
alert tcp any any -> any any (msg:"Test TCP Alert"; sid:1000003;)
