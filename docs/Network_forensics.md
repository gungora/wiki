**Network forensics** is the process of capturing information that moves
over a [network](network "wikilink") and trying to make sense of it in
some kind of forensics capacity. A [network forensics
appliance](network_forensics_appliance "wikilink") is a device that
automates this process.

There are both open source and proprietary network forensics systems
available.

## Overview

| System                                  | [License](software_license "wikilink") | User Interface                                                          | Supported Platform                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Supported Protocols                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Refs    |     |     |
|-----------------------------------------|----------------------------------------|-------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------|-----|-----|
| [Argus](Argus "wikilink")               | [Open Source](Open_Source "wikilink")  | Command Line, GUI via [ArgusEye](http://www.datenspionage.de/arguseye/) | Mac OS X, Linux, Solaris, FreeBSD, OpenBSD, NetBSD, AIX, IRIX, Windows (under Cygwin) and OpenWrt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | L2 addresses, tunnel identifiers (MPLS, GRE, ESP, etc...), protocol ids, SAP's, hop-count, options, L4 transport identification (RTP, RTCP detection), host flow control indication; netflow                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |         |     |     |
| [Chaosreader](Chaosreader "wikilink")   | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Solaris, RedHat, Windows                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | FTP files, HTTP transfers (HTML, GIF, JPEG, ...), SMTP emails, ... from the captured data inside network traffic logs                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |         |     |     |
| [DataEcho](DataEcho "wikilink")         | [Open Source](Open_Source "wikilink")  | GUI                                                                     | Windows                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | www, http                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |         |     |     |
| [Junkie](Junkie "wikilink")             | [Open Source](Open_Source "wikilink")  | GUI                                                                     | unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |         |     |     |
| [kisMAC](kisMAC "wikilink")             | [Open Source](Open_Source "wikilink")  | GUI                                                                     | Mac OS X, Linux, Solaris, FreeBSD, OpenBSD, NetBSD, AIX, IRIX, Windows (under Cygwin) and OpenWrt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | L2 addresses, tunnel identifiers (MPLS, GRE, ESP, etc...), protocol ids, SAP's, hop-count, options, L4 transport identification (RTP, RTCP detection), host flow control indication; netflow                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |         |     |     |
| [kismet](kismet "wikilink")             | [Open Source](Open_Source "wikilink")  | Command Line /GUI via [ArgusEye](http://www.datenspionage.de/arguseye/) | Mac OS X                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |         |     |     |
| [n2disk](n2disk "wikilink")             | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Ubuntu, CentOS                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |         |     |     |
| [net-sniff-ng](net-sniff-ng "wikilink") | [Open Source](Open_Source "wikilink")  | unknown                                                                 | unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |         |     |     |
| [netfse](netfse "wikilink")             | [Open Source](Open_Source "wikilink")  | GUI                                                                     | unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | TCP/IP, UDP                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |         |     |     |
| [netsleuth](netsleuth "wikilink")       | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Windows, [Backtrack](Backtrack "wikilink")                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Apple MDNS / Bonjour, SMB / CIFS / NetBios, DHCP (using the www.fingerbank.org resource), SSDP (as used in Microsoft Zero Config)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |         |     |     |
| [NetworkMiner](NetworkMiner "wikilink") | [Open Source](Open_Source "wikilink")  | Windows GUI, Commandline                                                | Linux / Mac OS X / FreeBSD, Windows                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | http, smb, ftp, tfpt, ssl , tls, tor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |         |     |     |
| [ntop](ntop "wikilink")                 | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Unix (including Linux, \*BSD, Solaris, and MacOSX), linux, windows                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | DPI via OpenDPI Library; FTP POP SMTP IMAP DNS IPP HTTP MDNS NTP NFS SSDP BGP SNMP XDMCP SMB SYSLOG DHCP PostgreSQL MySQL TDS DirectDownloadLink I23V5 AppleJuice DirectConnect Socrates WinMX MANOLITO PANDO Filetopia iMESH Kontiki OpenFT Kazaa/Fasttrack Gnutella eDonkey Bittorrent (Extended) OFF AVI Flash OGG MPEG QuickTime RealMedia Windowsmedia MMS XBOX QQ MOVE RTSP Feidian Icecast PPLive PPStream Zattoo SHOUTCast SopCast TVAnts TVUplayer VeohTV QQLive Thunder/Webthunder Soulseek GaduGadu IRC Popo Jabber MSN Oscar Yahoo Battlefield Quake Second Life Steam Halflife2 World of Warcraft Telnet STUN IPSEC GRE ICMP IGMP EGP SCTP OSPF IP in IP RTP RDP VNC PCAnywhere SSL SSH USENET MGCP IAX TFTP |         |     |     |
| [OSSEC](OSSEC "wikilink")               | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Windows 7, XP, 2000 and Vista Windows Server 2003 and 2008 VMWare ESX 3.0,3.5 (including CIS checks) FreeBSD (all versions) OpenBSD (all versions) NetBSD (all versions) Solaris 2.7, 2.8, 2.9 and 10 AIX 5.3 and 6.1 HP-UX 10, 11, 11i MacOSX 10 remote syslog: Cisco PIX, ASA and FWSM (all versions) Cisco IOS routers (all versions) Juniper Netscreen (all versions) SonicWall firewall (all versions) Checkpoint firewall (all versions) Cisco IOS IDS/IPS module (all versions) Sourcefire (Snort) IDS/IPS (all versions) Dragon NIDS (all versions) Checkpoint Smart Defense (all versions) McAfee VirusScan Enterprise (v8 and v8.5) Bluecoat proxy (all versions) Cisco VPN concentrators (all versions) Database monitoring is available for the following systems: MySQL (all versions) PostgreSQL (all versions) Oracle, MSSQL (to be available soon)" | Unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |         |     |     |
| [Snort](Snort "wikilink")               | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Linux, Windows                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Unknown                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |         |     |     |
| [Wireshark](Wireshark "wikilink")       | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Windows, Linux, Mac OS X, Solaris, FreeBSD, NetBSD, and others                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | IPsec, ISAKMP, Kerberos, SNMPv3, SSL/TLS, WEP, and WPA/WPA2; Wireshark can decrypt IEEE 802.11 WLAN data with user specified encryption keys, and others                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |         |     |     |
| [xplico](xplico "wikilink")             | [Open Source](Open_Source "wikilink")  | Command Line, GUI                                                       | Linux                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | ARP Radiotap Ethernet PPP VLAN L2TP IPv4 IPv6 TCP UDP DNS HTTP SMTP POP IMAP SIP MGCP H323 RTP RTCP SDP FB chat FTP IPP CHDLC PJL NNTP MSN IRC YAHOO GTALK EMULE SSL/TLS IPsec 802.11 LLC MMSE Linux cooked TFTP SNOOP PPPoE Telnet WebMail Paltalk Exp. Paltalk NetBIOS SMB PPI syslog G711ulaw, G711alaw, G722, G729, G723, G726 and RTAudio (x-msrta: Real Time Audio).                                                                                                                                                                                                                                                                                                                                                | Unknown |     |     |
| System                                  | [License](software_license "wikilink") | User Interface                                                          | Supported Platform                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Supported Protocols                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Refs    |     |     |

## Tips and Tricks

- The time between two events triggered by an intruder (as seen in
  logfiles, for example) can be helpful. If it is very short, you can be
  pretty sure that the actions were performed by an automated script and
  not by a human user.

## See also

- [Wireless forensics](Wireless_forensics "wikilink")
- [SSL forensics](SSL_forensics "wikilink")

<!-- -->

- [IP geolocation](IP_geolocation "wikilink")
- [Tools:Network Forensics](Tools:Network_Forensics "wikilink")
- [Tools:Logfile Analysis](Tools:Logfile_Analysis "wikilink")

## External links

- [Default Time To Live (TTL)
  values](http://www.binbert.com/blog/2009/12/default-time-to-live-ttl-values/)
- [http2 explained](http://daniel.haxx.se/http2/), by Daniel Stenberg,
  February 18, 2015

## Tools

### Open Source Network Forensics

- [Argus](Argus "wikilink")
- [Bulk Extractor](Bulk_Extractor "wikilink")
  [1](https://github.com/simsong/bulk_extractor)
- [Chaosreader](Chaosreader "wikilink") is a session reconstruction tool
  (supports both live or captured network traffic)
- [DataEcho](DataEcho "wikilink")
- [FlowGREP](FlowGREP "wikilink") is a basic IDS/IPS tool written in
  python [2](http://www.monkey.org/~jose/software/flowgrep/)
- [KisMAC](KisMAC "wikilink") is a free, open source wireless stumbling
  and security tool for Mac OS X. [3](http://kismac-ng.org)
- [Kismet](Kismet "wikilink")
- [logstash](logstash "wikilink") is a tool for managing events and
  logs. You can use it to collect logs, parse them, and store them for
  later use (like, for searching). Speaking of searching, logstash comes
  with a web interface for searching and drilling into all of your logs.
  [4](http://logstash.net/)

<!-- -->

- [log2Timeline](log2Timeline "wikilink") a framework for automatic
  creation of a super timeline. The main purpose is to provide a single
  tool to parse various log files and artifacts found on suspect systems
  (and supporting systems, such as network equipment) and produce a
  timeline that can be analysed by forensic investigators/analysts.
  [5](https://code.google.com/p/log2timeline/)
- [NetFSE](NetFSE "wikilink") is a web-based search and analysis
  application for high-volume network data [available at
  NetFSE.org](http://www.netfse.org)
- [NetSleuth](http://www.netgrab.co.uk) is a live and retrospective
  network analysis and triage tool.
- [ntop](ntop "wikilink")
- [NetGREP](NetGREP "wikilink") is a command line tool which tells you
  which lines in a text file contain network resources related to a
  particular country or Autonomous Network (AS)
  [6](https://pypi.python.org/pypi/netgrep/)
- [NetworkMiner](NetworkMiner "wikilink") is [an open source Network
  Forensics Tool available at
  SourceForge](http://sourceforge.net/apps/mediawiki/networkminer/index.php?title=NetworkMiner)
- [OSSEC](OSSEC "wikilink")
- [Plaso](Plaso "wikilink") (plaso langar að safna öllu) is the Python
  based back-end engine used by tools such as log2timeline for automatic
  creation of a super timelines [7](http://plaso.kiddaland.net/)

<!-- -->

- [RegRipper](RegRipper "wikilink") is an open source tool, written in
  Perl, for extracting/parsing information (keys, values, data) from the
  Registry and presenting it for analysis
  [8](http://regripper.wordpress.com/)
- [Snort](Snort "wikilink")
- [Wireshark](Wireshark "wikilink")
- [Xplico](Xplico "wikilink") is an Internet/IP Traffic Decoder (NFAT).
  Protocols supported: [HTTP, SIP, FTP, IMAP, POP, SMTP, TCP, UDP, IPv4,
  IPv6, ...](http://www.xplico.org/status.html)

### Commercial Network Forensics

#### Deep-Analysis Systems

- Code Green Networks [Content Inspection
  Appliance](http://www.codegreennetworks.com) - Passive monitoring and
  mandatory proxy mode. Easy to use Web GUI. Linux platform. Uses
  Stellent Outside In to access document content and metadata.
- E-Detective [9](http://www.edecision4u.com/)
  [10](http://www.digi-forensics.com/home.html)
- [InfoWatch Traffic Monitor](http://www.infowatch.com)
- Mera Systems [NetBeholder](http://netbeholder.com/)
- MFI Soft [SORMovich](http://sormovich.ru/) (in Russian)
- Solera Networks - Provider of full packet capture network forensics
  appliances [Solera Networks](http://www.soleranetworks.com/)
- NETRESEC [NetworkMiner Professional (portable network forensic
  analysis tool for
  Windows)](http://www.netresec.com/?page=NetworkMiner)
- NetWitness Corporation - Freeware/Commercial, Enterprise-Wide,
  Real-Time Network Forensics [NetWitness](http://www.netwitness.com/)
- Network Instruments [11](http://www.networkinstruments.com/)
- NIKSUN's [NetDetector](NetDetector "wikilink")
- PacketMotion [12](http://www.packetmotion.com/)
- Sandstorm's
  [NetIntercept](http://www.sandstorm.net/products/netintercept/) -
  Passive monitoring appliance. Qt/X11 GUI. FreeBSD platform. Uses
  forensic parsers written by Sandstorm to access document content and
  metadata.
- WildPackets [OmniPeek](OmniPeek "wikilink")
  [13](http://www.wildpackets.com/solutions/it_solutions/network_forensics)
  [14](http://www.wildpackets.com/products/distributed_network_analysis/omnipeek_network_analyzer/forensics_search)
- [Xplico](Xplico "wikilink") [15](http://www.xplico.org/)
- Expert Team - 3i System [16](http://www.expert-team.net/)

#### Flow-Based Systems

- Arbor Networks
- CapAnalysis [17](http://www.capanalysis.net/)
- GraniteEdge Networks
- Lancope <http://www.lancope.com/>
- Mantaro Product Development Services
  <http://www.mantaro.com/products/MNIS/index.htm>
- Mazu Networks <http://www.mazunetworks.com/>

#### Hybrid Systems

These systems combine flow analysis, deep analysis, and security event
monitoring and reporting.

- Q1 Labs <http://www.q1labs.com/>

[Category:Network Forensics](Category:Network_Forensics "wikilink")