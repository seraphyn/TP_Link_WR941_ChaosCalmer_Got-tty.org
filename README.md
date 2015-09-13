# TP_Link_WR941_ChaosCalmer_Got-tty.org
Created images of openwrt chaos calmer 15.05 für TP-Link WR941ND Version 5.1

See Article at https://got-tty.org for more information

https://openwrt.org/

Changelog from openwrt Chaos Calmer 15.05

** Highlights since Barrier Breaker **
* Linux kernel updated to version 3.18
* Improved Security Features
    - Rewritten package signing architecture based on ed25519
    - Added support for jails
    - Added support for hardened builds
* Improved Networking Support
    - Added or improved support for lots of 3G/4G modems (MBIM, QMI, NCM, ...)
    - Added support for 464XLAT (CLAT) [RFC 6877 + RFC 7050]
    - Netfilter performance enhancements (conntrack route cache)
    - Improved support for self-managing networks [draft-ietf-homenet-hncp]
    - Better multi-core support for the network stack
    - Improved support for MAP-E, MAP-T and LW4over6 IPv4 transitioning technologies
        [draft-ietf-softwire-map, -map-t, -map-dhcp, -lw4over6]
    - Improved network auto-setup capable of detecting and bootstrapping IPv4-only,
      6rd, Dual-Stack, IPv6-only, DS-Lite, LW4over6, MAP-E, MAP-T, 464XLAT
      and combinations without explicit configuration [based on RFC 7084]
    - Added support for Smart Queue Management (SQM) QoS, AQM and Traffic Shaping
    - Improved support for DNSSEC
* Platform and Driver Support
    - Added support for feeds of externally maintained targets
    - New mt7621 subtarget for Mediatek 11ac SoC
    - New mt76 mac80211 based wifi driver for MTK 11ac cores.
    - New mwlwifi mac80211 based wifi driver for the Marvell 88W8864
    - New bcm53xx target for Broadcom ARM BCM47xx/53xx devices
    - New mxs target for Freescale i.MX23/28 family and various boards
    - New sunxi target for AllWinner A10/A13/A20 family and various boards
    - brcm2708: support for Raspberry Pi 2
    - brcm63xx: support for BCM6318 and BCM63268 family
    - brcm63xx: improved fallback sprom support with bcma support

** Improvements since RC 3 **
* Updated 3.18 to 3.18.20
* Security update of openssl to 1.0.2d
* Security update of curl
* brcmfmac: many BCM43602 related fixes
* ar71xx: support more devices
* brcm47xx/bcm53xx: support any NVRAM size
* bcm53xx: basic Netgear R7000 support & R8000 image
** Improvements since RC 2 **
* brcmfmac: support for BCM43602
* mt76: updated version with new firmware support, TX & DMA fixes
* Updated 3.18 to 3.18.17
* Fixed image builder generation
* Various security updates (e.g. openssl, curl)
* Minor fixes
** Improvements since RC 1 **
* Fixed broken ImageBuilders for most targets
* Updated 3.18 to 3.18.14
* Fixed broken IPv6 downstream DHCPv6-PD and onlink-route handling
* Images (special format) for Asus brcm47xx and bcm53xx devices
* Improved stability of sysupgrade on brcm47xx and bcm53xx
* Added HTTPS enforcement option to uhttpd
* Fixed umask issue
* Added support for a few new boards
And lots and lots of other advancements...
As always a big thank you goes to all our active package maintainers, testers, supporters and documenters.
