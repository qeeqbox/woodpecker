<p align="center"> <img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/woodpecker.png"></p>

#
[![Generic badge](https://img.shields.io/badge/dynamic/json.svg?url=https://raw.githubusercontent.com/qeeqbox/woodpecker/master/info&label=Woodpecker&query=$.woodpecker&colorB=blue&style=flat-square)](https://github.com/qeeqbox/woodpecker/blob/master/changes.md) [![Generic badge](https://img.shields.io/static/v1?label=%F0%9F%91%8D&message=!&color=yellow&style=flat-square)](https://github.com/qeeqbox/woodpecker/stargazers)

Woodpecker is a custom security distro for remote penetration testing. Some of the original woodpecker's tools are replaced with newer ones (Tor and VPN initializers). This specific variation is based on Ubuntu and easy to maintain. 

## Screenshot
<img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/intro.gif" style="max-width:768px"/>

<img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/intro.png" style="max-width:768px"/>

## Revamped Features
#### Tor and VPN integrated in the desktop right click menu
<img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/menu.png" style="max-width:768px"/>

#### IP box in the desktop tray
<img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/ip.png" style="max-width:768px"/>

#### IP box stats the desktop tray
<img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/ipstats.png" style="max-width:768px"/>

#### System and network information on the desktop
<img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/system.png" style="max-width:768px"/>

#### Current logs are displyed on the desktop
<img src="https://raw.githubusercontent.com/qeeqbox/woodpecker/master/readme/logs.png" style="max-width:768px"/>

## Running
```console 
docker run -it --cap-add=NET_ADMIN qeeqbox/woodpecker:1.0
...
...
Successfully built 20055ad080f9
Successfully tagged qeeqbox/woodpecker:1.0

https://github.com/qeeqbox/woodpecker

Custom Woodpecker Security distro for pentesting

[>] Init
[>] Setting root password
[>] Setting xuser password
[>] Setting up vnc 1-4
[>] Setting up vnc 2-4
[>] Setting up vnc 3-4
[>] Setting up vnc 4-4
[>] Localhost exists
[>] Init qnetwork
[>] Setup tor 1-1 None
[>] Setup openvpn.. 1-1 Done

root pass -> lS8OjqpR66
-----------------------
Username  -> xuser
Password  -> RMy3^NX;AZ
VNC pass  -> x#<q!J<thS

http://172.17.0.2:6080/index.html
```

For pre IP or DNS configuration (Usfual in some)

```console 
docker run -it --cap-add=NET_ADMIN qeeqbox/woodpecker:1.0 "IP Address or none" "DNS list or non"
docker run -it --cap-add=NET_ADMIN qeeqbox/woodpecker:1.0 none "nameserver 8.8.4.4"
```

## Issues
#### Tor or VPN is stuck on initializing
Right click -> Application -> Qbox tools -> Disable the service and then Enable it (Read the logs from on the desktop)

#### Some logs do not show up
Right click -> Application -> Qbox tools -> Rest logs

## Changing resolution
- RDP (Change it using the clint app)
- VNC (Change it using right click -> resolution or use `xrandr -s ...`)
- Web browser Change it using right click -> resolution or use `xrandr -s ...`)

## Installed tools
afflib-tools aircrack-ng apktool arping arp-scan arpwatch autopsy backdoor-factory bbqsql bdfproxy binwalk bluez bluez-hcidump braa btscanner cabextract cadaver cewl cgpt cherrytree chirp chkrootkit chntpw clang cmospwd crunch cryptcat cryptsetup curlftpfs cutycapt darkstat dc3dd dcfldd dhcpig dirb dmitry dns2tcp dnsrecon dnstracer dnswalk doona dos2unix driftnet dsniff edb-debugger ethtool ettercap-common ettercap-dbg ettercap-graphical ewf-tools exiv2 extundelete fcrackzip flasm foremost fping funkload galleta gdb ghex guymager hackrf hashcat hashdeep hashid hping3 httrack hydra hydra-gtk i2c-tools ifenslave ike-scan inetsim iodine john kismet leafpad libfreefare-bin libhivex-bin libnfc-bin lynis macchanger magicrescue maskprocessor masscan mc mdbtools mdk3 medusa memdump minicom miredo missidentify mitmproxy nasm nbtscan ncrack ncurses-hexedit netdiscover netmask netsed netsniff-ng netwag ngrep nikto nmap onesixtyone ophcrack ophcrack-cli p0f pasco patator pdfcrack pev pixiewps polenum proxychains proxytunnel pst-utils ptunnel pyrit python-impacket python-scapy radare2 rake reaver recon-ng recordmydesktop recoverjpeg redsocks reglookup rifiuti rifiuti2 safecopy samdump2 sbd scalpel scrounge-ntfs sendemail siege sipcrack skipfish sleuthkit socat spectools sqlitebrowser sqlmap ssldump sslh sslscan sslscan kismet sslsniff sslsplit sslstrip statsprocessor stunnel4 suckless-tools sucrack swaks t50 tcpdump tcpflow tcpick tcpreplay thc-ipv6 udptunnel vboot-kernel-utils vboot-utils vim-gtk vinetto vlan volatility vpnc wafw00f wapiti wfuzz whatweb wifite wireshark xpdf xprobe xtightvncviewer yersinia zenmap zim zmap

## Roadmap
- ~~Add IP argument~~
- ~~Add DNS option (Requested)~~
- ~~Qemu image~~
- ~~Add VPN country option (Requested)~~
- ~~Stabilized qtools and changed default browser~~
- Add Brave (Requested)

## Official images (Not custom ones)
- [Ubuntu](https://ubuntu.com/)

## Licncess
- https://ubuntu.com/licensing
- https://github.com/torproject/tor/blob/master/LICENSE
- https://www.vpngate.net/en/join.aspx
- https://wiki.xfce.org/faq
- https://github.com/numixproject/numix-icon-theme/blob/master/license

## Articles
[raidforums](https://raidforums.com/Thread-Woodpecker-security-distro-for-remote-penetration-testing) [esgeeks](https://esgeeks.com/woodpecker-distro-seguridad-pentesting/?feed_id=1588&_unique_id=5f848450cba14)

## Disclaimer\Notes
- Treat this image as server
- Do not deploy without proper configuration
- Setup some security group rules and remove default credentials

## Other Projects
[![](https://github.com/qeeqbox/.github/blob/main/data/social-analyzer.png)](https://github.com/qeeqbox/social-analyzer) [![](https://github.com/qeeqbox/.github/blob/main/data/analyzer.png)](https://github.com/qeeqbox/analyzer) [![](https://github.com/qeeqbox/.github/blob/main/data/chameleon.png)](https://github.com/qeeqbox/chameleon) [![](https://github.com/qeeqbox/.github/blob/main/data/honeypots.png)](https://github.com/qeeqbox/honeypots) [![](https://github.com/qeeqbox/.github/blob/main/data/url-sandbox.png)](https://github.com/qeeqbox/url-sandbox) [![](https://github.com/qeeqbox/.github/blob/main/data/mitre-visualizer.png)](https://github.com/qeeqbox/mitre-visualizer) [![](https://github.com/qeeqbox/.github/blob/main/data/docker-images.png)](https://github.com/qeeqbox/docker-images) [![](https://github.com/qeeqbox/.github/blob/main/data/seahorse.png)](https://github.com/qeeqbox/seahorse) [![](https://github.com/qeeqbox/.github/blob/main/data/rhino.png)](https://github.com/qeeqbox/rhino)
