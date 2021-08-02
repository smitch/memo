# ex
- [EX4300 Switches Hardware Overview](https://www.juniper.net/documentation/en_US/release-independent/junos/topics/topic-map/ex4300-system-overview.html#ex4300-hardware-overview)
- [junos routing elementary PDF](https://www.juniper.net/jp/jp/local/pdf/others/jre.pdf)
- [ネットワーク管理システムへの MIB ファイルのロード](https://www.juniper.net/documentation/ja/junos/topics/task/operational/mib-loadng-to-nms-junos-nm.html)
-   [Configuring a Recursive DNS Server Address for IPv6 Hosts](https://www.juniper.net/documentation/us/en/software/junos/icmp/topics/task/recursive-dns-server-address-ipv6-configuring.html)
- [data sheet PDF](https://www.juniper.net/assets/jp/jp/local/pdf/datasheets/1000467-en.pdf)
- [Example: Configuring IPv6 Interfaces and Enabling Neighbor Discovery](https://www.juniper.net/documentation/en_US/junos/topics/topic-map/ipv6-interfaces-neighbor-discovery.html#id-example-configuring-ipv6-interfaces-and-enabling-neighbor-discovery)
-   [DHCP サーバーとしてのスイッチの設定 (CLI プロシージャ)](https://www.juniper.net/documentation/ja/junos/topics/topic-map/dhcp-for-switching-devices.html#id-configuring-a-switch-as-a-dhcp-server-cli-procedure)
- [インターフェイス名の物理部](https://www.juniper.net/documentation/ja/junos/topics/concept/interfaces-interface-naming-overview.html#id-10147130)
- [Juniper EXのSplit and Merge機能の功罪](https://blog.sidetech.jp/2014/12/05/182257)
- [Junos OS用語集](https://www.hs-juniperproducts.jp/guide/junos_words/word.html)
-   [Configuring the IPFIX Template Properties](https://www.juniper.net/documentation/us/en/software/junos/flow-monitoring/topics/concept/services-ipfix-flow-template-flow-aggregation-configuring.html#configuring-inline-j-flow-to-use-ipfix-flow-templates-on-mx-vmx-and-t-series-routers-ex-series-switches-nfx-series-devices-and-srx-devices__id-11332295)
- [Difference Jflow, Cflow and Netflow](https://community.juniper.net/communities/community-home/digestviewer/viewthread?MID=73286)
- [8. VLAN Pooling](https://qiita.com/tokuhy/items/013e5d7ab1c2c17129dd#8-vlan-pooling)
- [junos upgrade](https://www.infraeye.com/study/junos6.html)
- [リンクアグリゲーション(802.3ad)の仕組み 〜負荷分散,LACPとStaticの違い](https://milestone-of-se.nesuke.com/nw-basic/link-aggregation/802-1ax/)
- [静的よりもLACPの方がよい理由](https://network.oreda.net/device/switch/lag.html#%E9%9D%99%E7%9A%84%E3%82%88%E3%82%8A%E3%82%82lacp%E3%81%AE%E6%96%B9%E3%81%8C%E3%82%88%E3%81%84%E7%90%86%E7%94%B1)
- [Configuring PoE Interfaces](https://www.juniper.net/documentation/us/en/software/junos/poe/topics/topic-map/poe-ex-series-configuring.html#id-configuring-poe-interfaces)
- [junos hands on training PDF](https://www.juniper.net/assets/jp/jp/local/pdf/additional-resources/junos-switching-training-ex-qfx-course-jp.pdf)
- [SRX シリーズ スタディガイド － パート 1](https://www.juniper.net/assets/jp/jp/local/pdf/others/JNCIS-SEC-1_.pdf)
- [Configuring an EX2300, EX3400, EX4300, or EX4400 Virtual Chassis with a Preprovisioned Configuration File](https://www.juniper.net/documentation/us/en/software/junos/virtual-chassis-qfx/topics/task/virtual-chassis-ex4300-configuring.html#id-configuring-an-ex4300-virtual-chassis-with-a-preprovisioned-configuration-file)
- [JUNOS_VirtualChassis](https://klock-3rd.hatenablog.com/entry/2018/06/30/225641)
- [Juniper SRX 日本語マニュアル 1. Junos OS インストール&アップグレード](https://www.juniper.net/assets/jp/jp/local/pdf/additional-resources/junos-installation-upgrade.pdf)
- [EXスタートアップガイド Virtual Chassis編](https://www.juniper.net/assets/jp/jp/local/pdf/additional-resources/exstartup-guide-vc-rev1-202101.pdf)
- [Understanding the Algorithm Used to Hash LAG Bundle and Egress Next-Hop ECMP Traffic](https://www.juniper.net/documentation/us/en/software/junos/interfaces-ethernet-switches/topics/topic-map/switches-interface-aggregated.html#id-understanding-the-algorithm-used-to-hash-lag-bundle-and-egress-nexthop-ecmp-traffic)
- [SRX シャーシクラスター 《ブランチ編》PDF](https://www.juniper.net/assets/jp/jp/local/pdf/others/br_chassis-clustering.pdf)
- [EX4300 イーサネット スイッチ ハードウェア 完全ガイド](https://www.juniper.net/documentation/ja/release-independent/junos/information-products/topic-collections/hardware/ex-series/ex4300/book-hw-ex4300.pdf)
- [Understanding Chassis Cluster Redundancy Groups](https://www.juniper.net/documentation/us/en/software/junos/chassis-cluster-security-devices/topics/topic-map/security-chassis-cluster-redundancy-groups.html#id-understanding-chassis-cluster-redundancy-groups)
- [show interfaces diagnostics optics](https://www.juniper.net/documentation/us/en/software/junos/flow-packet-processing/topics/ref/command/show-interfaces-diagnostics-optics-srx.html)
- [automatic (Source NAT Next Gen Services)](https://www.juniper.net/documentation/us/en/software/junos/interfaces-next-gen-services/topics/ref/statement/automatic-edit-services-nat-source-port-usf.html)

# nat port assignment
```
Automatic port assignment uses the port range 1024 through 65535.
```

# TCP/UDP timeout
```
デフォルトのタイムアウトは、TCP では 30 分、UDP では 1 分です。
```
# memo url only

- https://klock-3rd.hatenablog.com/entry/2018/08/09/234202
https://www.reddit.com/r/Juniper/comments/6a6253/ex3400_tagged_and_untagged_vlan_on_one_interface/
- https://nokonokonetwork.com/juniper/srx_cli_command_syslog_security_log.html
- https://nokonokonetwork.com/juniper/how_to_use_juniper_vlabs_for_free.html
- https://nokonokonetwork.com/juniper/how_to_resister_user_accout_for_private_use.html
- https://www.juniper.net/documentation/us/en/software/junos/utm/topics/ref/command/show-security-log.html
https://kb.juniper.net/InfoCenter/index?page=content&id=KB16509
- https://www.juniper.net/documentation/en_US/release-independent/nce/topics/task/operational/chassis-cluster-srx-log-message-configuring.html
- https://www.juniper.net/documentation/ja/junos/topics/task/configuration/interfaces-enabling-or-disabling-snmp-notifications-on-logical-interfaces.html
- https://www.juniper.net/documentation/us/en/software/junos/network-mgmt/topics/ref/statement/security-edit-stream-security-log.html
- https://www.juniper.net/documentation/en_US/junos/topics/task/configuration/security-system-stream-security-log-revenue-port-setting.html
- https://kb.juniper.net/InfoCenter/index?page=content&id=KB16506&actp=METADATA
- https://www.juniper.net/documentation/us/en/software/junos/virtual-chassis-mx/topics/ref/command/request-virtual-chassis-routing-engine-master-switch-mx-series.html
- https://www.infraeye.com/study/srx8.html
- https://www.juniper.net/documentation/en_US/junos/topics/reference/configuration-statement/source-address-edit-system-ntp-radius-syslog-tacacs.html
- https://itengine.seesaa.net/article/457187173.html
- https://kb.juniper.net/InfoCenter/index?page=content&id=KB21563&actp=METADATA
- https://www.infraexpert.com/study/catalyst25.html
- 

https://blog.daichang.me/?p=364
https://www.juniper.net/documentation/ja/junos/topics/task/configuration/syslog-specifying-message-facility-and-severity.html
https://www.juniper.net/documentation/ja/junos/topics/task/configuration/syslog-alternative-facility-name-remote-messages-configuring.html
https://www.juniper.net/documentation/ja/junos/topics/example/snmp-config-cli-qfx-series.html
https://nwengblog.com/srx-mngfilter/
https://www.juniper.net/documentation/en_US/junos/topics/example/junos-cli-wildcard-range-configuring.html
https://www.slideshare.net/ZenSekibe/junos-junos-cli-216790357
https://www.slideshare.net/ZenSekibe/junos-dhcp
https://www.juniper.net/documentation/ja/junos/topics/task/configuration/ssh-services-configuring.html
https://community.juniper.net/communities/community-home/digestviewer/viewthread?MID=70700
https://gist.github.com/BlackMoonWolf/367a099f173c48d6eb36eb2445f358ed
https://www.juniper.net/documentation/en_US/junos13.2/topics/task/configuration/virtual-chassis-ex4300-configuring.html
https://www.juniper.net/documentation/jp/ja/software/junos/cli/topics/topic-map/synchronising-routing-engines.html
https://if-network.com/junos-commit-confirmed/
https://www.juniper.net/documentation/ja/junos/topics/task/operational/mib-loadng-to-nms-junos-nm.html
https://www.juniper.net/documentation/en_US/release-independent/topics/reference/specifications/frus-ex-series.pdf
https://www.juniper.net/documentation/us/en/software/license/licensing/topics/topic-map/understanding_software_licenses.html
https://www.juniper.net/documentation/ja/junos/topics/task/configuration/bridging-routed-vlan-interfaces-qfx-series-cli.html
https://www.juniper.net/documentation/us/en/software/junos/static-routing/topics/topic-map/config_static-routes.html#id-example-configuring-ipv6-static-routes
https://www.juniper.net/documentation/jp/ja/software/junos/cli/topics/ref/command/set-cli-screen-width-junos-cli.html
https://itengine.seesaa.net/article/465425254.html
https://www.juniper.net/documentation/jp/ja/software/junos/routing-policy/topics/example/firewall-filter-option-multiple-listed-example.html
https://www.juniper.net/documentation/ja/junos/topics/task/installation/virtual-chassis-ex4200-member-adding-cli.html
https://www.juniper.net/documentation/jp/ja/software/junos/cli/topics/topic-map/modifying-configuration.html#id-example-using-global-replace-in-a-junos-os-configuration-replacing-an-interface-name
https://www.juniper.net/documentation/ja/release-independent/junos/topics/task/configuration/ex-series-switch-default-factory-configuration-reverting.html
https://www.juniper.net/documentation/jp/ja/software/junos/routing-policy/topics/example/firewall-filter-option-multiple-listed-example.html
https://itengine.seesaa.net/article/440288166.html
https://www.juniper.net/documentation/us/en/software/junos/virtual-chassis-qfx/topics/task/virtual-chassis-ex4200.html
https://www.juniper.net/documentation/us/en/software/junos/virtual-chassis-fabric/topics/ref/command/request-virtual-chassis-mode-mixed-ex-series.html
https://www.juniper.net/documentation/us/en/software/junos/virtual-chassis-qfx/topics/task/virtual-chassis-ex4300-configuring.html
https://www.juniper.net/documentation/ja/junos/topics/topic-map/aggregated-ethernet-interfaces-lacp-configuring.html#id-example-configuring-aggregated-ethernet-interfaces
https://www.juniper.net/documentation/en_US/junos/topics/task/configuration/dns-name-server-configuring-qfx-series.html
https://qiita.com/suzuki-navi/items/2410ebdf92279996c516
https://changineer.info/server/monitoring/monitoring_snmptrapd.html#toc4
https://kb.juniper.net/InfoCenter/index?page=content&id=KB13641&actp=METADATA
https://qiita.com/hatman621221/items/7d220f78a820ec0ec8a1
https://sites.google.com/site/osscatalog/tips/linux/centos-snmptrapd-mib-add
http://www.usupi.org/info/pf.html
https://www.dragonflybsd.org/~aggelos/pf/ja/rdr.html
https://www.dragonflybsd.org/~aggelos/pf/ja/nat.html
https://www.atmarkit.co.jp/ait/articles/0109/29/news005.html
https://qiita.com/masa2223/items/65eb6df07c01e7ebda64
https://www.reddit.com/r/Juniper/comments/8u4055/release_all_ip_addresses_at_once/
https://www.juniper.net/documentation/ja/junos/topics/task/configuration/interfaces-interface-ranges-multi-task.html
https://community.juniper.net/communities/community-home/digestviewer/viewthread?MID=67981
https://www.juniper.net/documentation/en_US/release-independent/nce/topics/task/operational/chassis-cluster-srx-log-message-configuring.html

https://www.juniper.net/documentation/ja/junos/topics/example/bgp-advertise-peer-as.html
https://www.juniper.net/documentation/ja/junos/topics/example/port-mirroring-local-ex-series-l2.html
https://kb.juniper.net/InfoCenter/index?page=content&id=KB36138&cat=EX_Series&actp=LIST
https://milestone-of-se.nesuke.com/nw-basic/nat/nat-summary/
https://www.juniper.net/documentation/us/en/software/junos/interfaces-ethernet-switches/topics/ref/command/show-interfaces-diagnostics-optics-ex-series.html


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0Nzc1NTQ4NjIsMTgxMTU2MzExMyw2MD
A1NTQ1MzgsODU0NDM2MjA1LDExNDM3NTQ4MTksLTEyMTA5MzQw
OTMsLTEzMTE5MzYxMDcsNjA0MDU0MTU0LDk4Mjg3MzY1NCwtMT
MxMDkyNjI4Myw3NjU4NzU2MDYsLTc3MjQxNDA2OCwzMzc0MTUw
MDQsNDYzMzczMzAzXX0=
-->