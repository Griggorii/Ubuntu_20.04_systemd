# ubuntu_20.04_systemd
ubuntu , zfs , systemd , fb , 20.04

Ubuntu 20.04 backup original sytemd home folder command:

$ cd ~/ && sudo XZ_OPT=-9 tar -Jcvf systemd-original-backup.tar.xz /lib/systemd /etc/systemd && cd -

$ sudo rm -rf /lib/systemd /etc/systemd

$ sudo tar xvpf systemd_griggorii_modification_20.04.tar.xz -C /
