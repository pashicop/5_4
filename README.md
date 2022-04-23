# 5_4
# 1
```
pashi@pashi-docker:~/5_4/src/packer$ packer build centos-7-base.json 
yandex: output will be in this color.

==> yandex: Creating temporary RSA SSH key for instance...
==> yandex: Using as source image: fd8v9fc454c44fr6lngi (name: "centos-7-v20220314", family: "centos-7")
==> yandex: Use provided subnet id e9bs7kit3200cgon7v45
==> yandex: Creating disk...
==> yandex: Creating instance...
==> yandex: Waiting for instance with id fhm6ic36eoaghahg9uqf to become active...
    yandex: Detected instance IP: 51.250.1.177
==> yandex: Using SSH communicator to connect: 51.250.1.177
==> yandex: Waiting for SSH to become available...
==> yandex: Connected to SSH!
==> yandex: Provisioning with shell script: /tmp/packer-shell254781513
    yandex: Loaded plugins: fastestmirror
    yandex: Determining fastest mirrors
    yandex:  * base: mirror.reconn.ru
    yandex:  * extras: mirror.sale-dedic.com
    yandex:  * updates: mirror.reconn.ru
    yandex: Resolving Dependencies
    yandex: --> Running transaction check
    yandex: ---> Package expat.x86_64 0:2.1.0-12.el7 will be updated
    yandex: ---> Package expat.x86_64 0:2.1.0-14.el7_9 will be an update
    yandex: ---> Package kernel.x86_64 0:3.10.0-1160.62.1.el7 will be installed
    yandex: ---> Package kernel-tools.x86_64 0:3.10.0-1160.59.1.el7 will be updated
    yandex: ---> Package kernel-tools.x86_64 0:3.10.0-1160.62.1.el7 will be an update
    yandex: ---> Package kernel-tools-libs.x86_64 0:3.10.0-1160.59.1.el7 will be updated
    yandex: ---> Package kernel-tools-libs.x86_64 0:3.10.0-1160.62.1.el7 will be an update
    yandex: ---> Package microcode_ctl.x86_64 2:2.1-73.11.el7_9 will be updated
    yandex: ---> Package microcode_ctl.x86_64 2:2.1-73.13.el7_9 will be an update
    yandex: ---> Package openssl.x86_64 1:1.0.2k-24.el7_9 will be updated
    yandex: ---> Package openssl.x86_64 1:1.0.2k-25.el7_9 will be an update
    yandex: ---> Package openssl-libs.x86_64 1:1.0.2k-24.el7_9 will be updated
    yandex: ---> Package openssl-libs.x86_64 1:1.0.2k-25.el7_9 will be an update
    yandex: ---> Package python-perf.x86_64 0:3.10.0-1160.59.1.el7 will be updated
    yandex: ---> Package python-perf.x86_64 0:3.10.0-1160.62.1.el7 will be an update
    yandex: ---> Package rsyslog.x86_64 0:8.24.0-57.el7_9.1 will be updated
    yandex: ---> Package rsyslog.x86_64 0:8.24.0-57.el7_9.2 will be an update
    yandex: ---> Package tzdata.noarch 0:2021e-1.el7 will be updated
    yandex: ---> Package tzdata.noarch 0:2022a-1.el7 will be an update
    yandex: --> Finished Dependency Resolution
    yandex:
    yandex: Dependencies Resolved
    yandex:
    yandex: ================================================================================
    yandex:  Package               Arch       Version                     Repository   Size
    yandex: ================================================================================
    yandex: Installing:
    yandex:  kernel                x86_64     3.10.0-1160.62.1.el7        updates      50 M
    yandex: Updating:
    yandex:  expat                 x86_64     2.1.0-14.el7_9              updates      83 k
    yandex:  kernel-tools          x86_64     3.10.0-1160.62.1.el7        updates     8.2 M
    yandex:  kernel-tools-libs     x86_64     3.10.0-1160.62.1.el7        updates     8.1 M
    yandex:  microcode_ctl         x86_64     2:2.1-73.13.el7_9           updates     4.2 M
    yandex:  openssl               x86_64     1:1.0.2k-25.el7_9           updates     494 k
    yandex:  openssl-libs          x86_64     1:1.0.2k-25.el7_9           updates     1.2 M
    yandex:  python-perf           x86_64     3.10.0-1160.62.1.el7        updates     8.2 M
    yandex:  rsyslog               x86_64     8.24.0-57.el7_9.2           updates     622 k
    yandex:  tzdata                noarch     2022a-1.el7                 updates     501 k
    yandex:
    yandex: Transaction Summary
    yandex: ================================================================================
    yandex: Install  1 Package
    yandex: Upgrade  9 Packages
    yandex:
    yandex: Total download size: 82 M
    yandex: Downloading packages:
    yandex: Delta RPMs disabled because /usr/bin/applydeltarpm not installed.
    yandex: --------------------------------------------------------------------------------
    yandex: Total                                               25 MB/s |  82 MB  00:03
    yandex: Running transaction check
    yandex: Running transaction test
    yandex: Transaction test succeeded
    yandex: Running transaction
    yandex:   Updating   : 1:openssl-libs-1.0.2k-25.el7_9.x86_64                       1/19
    yandex:   Updating   : kernel-tools-libs-3.10.0-1160.62.1.el7.x86_64               2/19
    yandex:   Updating   : kernel-tools-3.10.0-1160.62.1.el7.x86_64                    3/19
    yandex:   Updating   : 1:openssl-1.0.2k-25.el7_9.x86_64                            4/19
    yandex:   Updating   : tzdata-2022a-1.el7.noarch                                   5/19
    yandex:   Installing : kernel-3.10.0-1160.62.1.el7.x86_64                          6/19
    yandex:   Updating   : expat-2.1.0-14.el7_9.x86_64                                 7/19
    yandex:   Updating   : 2:microcode_ctl-2.1-73.13.el7_9.x86_64                      8/19
    yandex:   Updating   : rsyslog-8.24.0-57.el7_9.2.x86_64                            9/19
    yandex:   Updating   : python-perf-3.10.0-1160.62.1.el7.x86_64                    10/19
    yandex:   Cleanup    : kernel-tools-3.10.0-1160.59.1.el7.x86_64                   11/19
    yandex:   Cleanup    : 1:openssl-1.0.2k-24.el7_9.x86_64                           12/19
    yandex:   Cleanup    : tzdata-2021e-1.el7.noarch                                  13/19
    yandex:   Cleanup    : 2:microcode_ctl-2.1-73.11.el7_9.x86_64                     14/19
    yandex:   Cleanup    : 1:openssl-libs-1.0.2k-24.el7_9.x86_64                      15/19
    yandex:   Cleanup    : kernel-tools-libs-3.10.0-1160.59.1.el7.x86_64              16/19
    yandex:   Cleanup    : expat-2.1.0-12.el7.x86_64                                  17/19
    yandex:   Cleanup    : rsyslog-8.24.0-57.el7_9.1.x86_64                           18/19
    yandex:   Cleanup    : python-perf-3.10.0-1160.59.1.el7.x86_64                    19/19
    yandex:   Verifying  : kernel-tools-libs-3.10.0-1160.62.1.el7.x86_64               1/19
    yandex:   Verifying  : 1:openssl-libs-1.0.2k-25.el7_9.x86_64                       2/19
    yandex:   Verifying  : 1:openssl-1.0.2k-25.el7_9.x86_64                            3/19
    yandex:   Verifying  : python-perf-3.10.0-1160.62.1.el7.x86_64                     4/19
    yandex:   Verifying  : rsyslog-8.24.0-57.el7_9.2.x86_64                            5/19
    yandex:   Verifying  : 2:microcode_ctl-2.1-73.13.el7_9.x86_64                      6/19
    yandex:   Verifying  : expat-2.1.0-14.el7_9.x86_64                                 7/19
    yandex:   Verifying  : kernel-3.10.0-1160.62.1.el7.x86_64                          8/19
    yandex:   Verifying  : tzdata-2022a-1.el7.noarch                                   9/19
    yandex:   Verifying  : kernel-tools-3.10.0-1160.62.1.el7.x86_64                   10/19
    yandex:   Verifying  : expat-2.1.0-12.el7.x86_64                                  11/19
    yandex:   Verifying  : kernel-tools-libs-3.10.0-1160.59.1.el7.x86_64              12/19
    yandex:   Verifying  : python-perf-3.10.0-1160.59.1.el7.x86_64                    13/19
    yandex:   Verifying  : tzdata-2021e-1.el7.noarch                                  14/19
    yandex:   Verifying  : 1:openssl-libs-1.0.2k-24.el7_9.x86_64                      15/19
    yandex:   Verifying  : kernel-tools-3.10.0-1160.59.1.el7.x86_64                   16/19
    yandex:   Verifying  : 2:microcode_ctl-2.1-73.11.el7_9.x86_64                     17/19
    yandex:   Verifying  : rsyslog-8.24.0-57.el7_9.1.x86_64                           18/19
    yandex:   Verifying  : 1:openssl-1.0.2k-24.el7_9.x86_64                           19/19
    yandex:
    yandex: Installed:
    yandex:   kernel.x86_64 0:3.10.0-1160.62.1.el7
    yandex:
    yandex: Updated:
    yandex:   expat.x86_64 0:2.1.0-14.el7_9
    yandex:   kernel-tools.x86_64 0:3.10.0-1160.62.1.el7
    yandex:   kernel-tools-libs.x86_64 0:3.10.0-1160.62.1.el7
    yandex:   microcode_ctl.x86_64 2:2.1-73.13.el7_9
    yandex:   openssl.x86_64 1:1.0.2k-25.el7_9
    yandex:   openssl-libs.x86_64 1:1.0.2k-25.el7_9
    yandex:   python-perf.x86_64 0:3.10.0-1160.62.1.el7
    yandex:   rsyslog.x86_64 0:8.24.0-57.el7_9.2
    yandex:   tzdata.noarch 0:2022a-1.el7
    yandex:
    yandex: Complete!
    yandex: Loaded plugins: fastestmirror
    yandex: Loading mirror speeds from cached hostfile
    yandex:  * base: mirror.reconn.ru
    yandex:  * extras: mirror.sale-dedic.com
    yandex:  * updates: mirror.reconn.ru
    yandex: Package iptables-1.4.21-35.el7.x86_64 already installed and latest version
    yandex: Package curl-7.29.0-59.el7_9.1.x86_64 already installed and latest version
    yandex: Package net-tools-2.0-0.25.20131004git.el7.x86_64 already installed and latest version
    yandex: Package rsync-3.1.2-10.el7.x86_64 already installed and latest version
    yandex: Package openssh-server-7.4p1-22.el7_9.x86_64 already installed and latest version
    yandex: Resolving Dependencies
    yandex: --> Running transaction check
    yandex: ---> Package bind-utils.x86_64 32:9.11.4-26.P2.el7_9.9 will be installed
    yandex: --> Processing Dependency: bind-libs-lite(x86-64) = 32:9.11.4-26.P2.el7_9.9 for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: bind-libs(x86-64) = 32:9.11.4-26.P2.el7_9.9 for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: liblwres.so.160()(64bit) for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: libisccfg.so.160()(64bit) for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: libisc.so.169()(64bit) for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: libirs.so.160()(64bit) for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: libdns.so.1102()(64bit) for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: libbind9.so.160()(64bit) for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: --> Processing Dependency: libGeoIP.so.1()(64bit) for package: 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64
    yandex: ---> Package bridge-utils.x86_64 0:1.5-9.el7 will be installed
    yandex: ---> Package tcpdump.x86_64 14:4.9.2-4.el7_7.1 will be installed
    yandex: --> Processing Dependency: libpcap >= 14:1.5.3-10 for package: 14:tcpdump-4.9.2-4.el7_7.1.x86_64
    yandex: --> Processing Dependency: libpcap.so.1()(64bit) for package: 14:tcpdump-4.9.2-4.el7_7.1.x86_64
    yandex: ---> Package telnet.x86_64 1:0.17-66.el7 will be installed
    yandex: --> Running transaction check
    yandex: ---> Package GeoIP.x86_64 0:1.5.0-14.el7 will be installed
    yandex: --> Processing Dependency: geoipupdate for package: GeoIP-1.5.0-14.el7.x86_64
    yandex: ---> Package bind-libs.x86_64 32:9.11.4-26.P2.el7_9.9 will be installed
    yandex: --> Processing Dependency: bind-license = 32:9.11.4-26.P2.el7_9.9 for package: 32:bind-libs-9.11.4-26.P2.el7_9.9.x86_64
    yandex: ---> Package bind-libs-lite.x86_64 32:9.11.4-26.P2.el7_9.9 will be installed
    yandex: ---> Package libpcap.x86_64 14:1.5.3-13.el7_9 will be installed
    yandex: --> Running transaction check
    yandex: ---> Package bind-license.noarch 32:9.11.4-26.P2.el7_9.9 will be installed
    yandex: ---> Package geoipupdate.x86_64 0:2.5.0-1.el7 will be installed
    yandex: --> Finished Dependency Resolution
    yandex:
    yandex: Dependencies Resolved
    yandex:
    yandex: ================================================================================
    yandex:  Package            Arch       Version                        Repository   Size
    yandex: ================================================================================
    yandex: Installing:
    yandex:  bind-utils         x86_64     32:9.11.4-26.P2.el7_9.9        updates     261 k
    yandex:  bridge-utils       x86_64     1.5-9.el7                      base         32 k
    yandex:  tcpdump            x86_64     14:4.9.2-4.el7_7.1             base        422 k
    yandex:  telnet             x86_64     1:0.17-66.el7                  updates      64 k
    yandex: Installing for dependencies:
    yandex:  GeoIP              x86_64     1.5.0-14.el7                   base        1.5 M
    yandex:  bind-libs          x86_64     32:9.11.4-26.P2.el7_9.9        updates     157 k
    yandex:  bind-libs-lite     x86_64     32:9.11.4-26.P2.el7_9.9        updates     1.1 M
    yandex:  bind-license       noarch     32:9.11.4-26.P2.el7_9.9        updates      91 k
    yandex:  geoipupdate        x86_64     2.5.0-1.el7                    base         35 k
    yandex:  libpcap            x86_64     14:1.5.3-13.el7_9              updates     139 k
    yandex:
    yandex: Transaction Summary
    yandex: ================================================================================
    yandex: Install  4 Packages (+6 Dependent packages)
    yandex:
    yandex: Total download size: 3.8 M
    yandex: Installed size: 9.0 M
    yandex: Downloading packages:
    yandex: --------------------------------------------------------------------------------
    yandex: Total                                               12 MB/s | 3.8 MB  00:00
    yandex: Running transaction check
    yandex: Running transaction test
    yandex: Transaction test succeeded
    yandex: Running transaction
    yandex:   Installing : 32:bind-license-9.11.4-26.P2.el7_9.9.noarch                 1/10
    yandex:   Installing : geoipupdate-2.5.0-1.el7.x86_64                              2/10
    yandex:   Installing : GeoIP-1.5.0-14.el7.x86_64                                   3/10
    yandex:   Installing : 32:bind-libs-lite-9.11.4-26.P2.el7_9.9.x86_64               4/10
    yandex:   Installing : 32:bind-libs-9.11.4-26.P2.el7_9.9.x86_64                    5/10
    yandex:   Installing : 14:libpcap-1.5.3-13.el7_9.x86_64                            6/10
    yandex: pam_tally2: Error opening /var/log/tallylog for update: Permission denied
    yandex: pam_tally2: Authentication error
    yandex: useradd: failed to reset the tallylog entry of user "tcpdump"
    yandex:   Installing : 14:tcpdump-4.9.2-4.el7_7.1.x86_64                           7/10
    yandex:   Installing : 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64                   8/10
    yandex:   Installing : bridge-utils-1.5-9.el7.x86_64                               9/10
    yandex:   Installing : 1:telnet-0.17-66.el7.x86_64                                10/10
    yandex:   Verifying  : GeoIP-1.5.0-14.el7.x86_64                                   1/10
    yandex:   Verifying  : 14:libpcap-1.5.3-13.el7_9.x86_64                            2/10
    yandex:   Verifying  : 1:telnet-0.17-66.el7.x86_64                                 3/10
    yandex:   Verifying  : 32:bind-libs-9.11.4-26.P2.el7_9.9.x86_64                    4/10
    yandex:   Verifying  : geoipupdate-2.5.0-1.el7.x86_64                              5/10
    yandex:   Verifying  : 14:tcpdump-4.9.2-4.el7_7.1.x86_64                           6/10
    yandex:   Verifying  : 32:bind-license-9.11.4-26.P2.el7_9.9.noarch                 7/10
    yandex:   Verifying  : bridge-utils-1.5-9.el7.x86_64                               8/10
    yandex:   Verifying  : 32:bind-libs-lite-9.11.4-26.P2.el7_9.9.x86_64               9/10
    yandex:   Verifying  : 32:bind-utils-9.11.4-26.P2.el7_9.9.x86_64                  10/10
    yandex:
    yandex: Installed:
    yandex:   bind-utils.x86_64 32:9.11.4-26.P2.el7_9.9   bridge-utils.x86_64 0:1.5-9.el7
    yandex:   tcpdump.x86_64 14:4.9.2-4.el7_7.1           telnet.x86_64 1:0.17-66.el7
    yandex:
    yandex: Dependency Installed:
    yandex:   GeoIP.x86_64 0:1.5.0-14.el7
    yandex:   bind-libs.x86_64 32:9.11.4-26.P2.el7_9.9
    yandex:   bind-libs-lite.x86_64 32:9.11.4-26.P2.el7_9.9
    yandex:   bind-license.noarch 32:9.11.4-26.P2.el7_9.9
    yandex:   geoipupdate.x86_64 0:2.5.0-1.el7
    yandex:   libpcap.x86_64 14:1.5.3-13.el7_9
    yandex:
    yandex: Complete!
==> yandex: Stopping instance...
==> yandex: Deleting instance...
    yandex: Instance has been deleted!
==> yandex: Creating image: centos-7-base
==> yandex: Waiting for image to complete...
==> yandex: Success image create...
==> yandex: Destroying boot disk...
    yandex: Disk has been deleted!
Build 'yandex' finished after 6 minutes 19 seconds.

==> Wait completed after 6 minutes 19 seconds

==> Builds finished. The artifacts of successful builds are:
--> yandex: A disk image was created: centos-7-base (id: fd8s077b0jo0r1k3j94c) with family name centos
pashi@pashi-docker:~/5_4/src/terraform$ yc compute image list
+----------------------+---------------+--------+----------------------+--------+
|          ID          |     NAME      | FAMILY |     PRODUCT IDS      | STATUS |
+----------------------+---------------+--------+----------------------+--------+
| fd8s077b0jo0r1k3j94c | centos-7-base | centos | f2esd9f5o5i9p7pkkk8k | READY  |
+----------------------+---------------+--------+----------------------+--------+


```
# 2
file:///home/pashi/Pictures/Screenshot%20from%202022-04-24%2000-33-05.png![image](https://user-images.githubusercontent.com/97126500/164946626-1be2bda7-2c6a-4a20-811d-fb3a2b2d0c57.png)
