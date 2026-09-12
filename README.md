Hardened DMZ Game Server

Defense-in-depth network architecture on enterprise Cisco hardware — routed DMZ, segmented VLANs, default-deny egress.

A production-style, physically segmented game server deployment built on a Cisco 1921 ISR, ASA 5515-X firewall, and Catalyst 2960X switch. Documented from cable trace to control validation.

Show Image


At a glance
	
Role	Network and security design, build, hardening, documentation
Edge router	Cisco 1921 ISR — NAT overload, edge ACL, QoS
Firewall	Cisco ASA 5515-X — three-legged: inside / dmz / outside
Switch	Cisco Catalyst WS-C2960X-48LPS-L — VLAN segmentation, L2 hardening
Server host	<CPU> / <RAM> / <DISK> — <OS + VERSION>
Exposed service	Minecraft Bedrock — UDP 19132, single-port static PAT
Users served	~5 allowlisted players
Key controls	Default-deny egress · DMZ→inside containment · VLAN segmentation with inter-VLAN ACLs · pull-based backups · single-port PAT · CVE triage via CISA KEV + EPSS
