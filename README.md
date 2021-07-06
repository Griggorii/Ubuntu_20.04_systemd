# ubuntu_20.04_systemd
ubuntu , zfs , systemd , fb , 20.04

Ubuntu 20.04 backup original sytemd home folder command:

$ cd ~/ && sudo XZ_OPT=-9 tar -Jcvf systemd-original-backup.tar.xz /lib/systemd /etc/systemd && cd -

$ sudo rm -rf /usr/lib/systemd /etc/systemd

$ sudo tar xvpf systemd_griggorii_modification_20.04.tar.xz -C /

$ sudo rm -rf '/usr/lib/systemd/user/busnames.target'

$ chmod -R a+rwx systemd-service-fstrim-on-upgrade-check-off

$ ./systemd-service-fstrim-on-upgrade-check-off

Reconfigure gdm3/lightdm/sddm just in case choose your option | на всякий случай выберите ваш вариант и пере деконфигурируйте

$ sudo dpkg-reconfigure gdm3

$ sudo dpkg-reconfigure lightdm

$ sudo dpkg-reconfigure sddm

Reboot

OS https://youtu.be/MVhZ_QZGxaQ
_______________________________________________________________________________________________________________________________________________________________

New glibc wayland not freeze https://github.com/Griggorii/glibc-2.31_all.deb_package_version_libc6-prof_2.31-0ubuntu9.2_amd64.deb_ubuntu_20.04_focal_fossa

Only real technologies, not any fictional parasitic distributions support real technology investments and donate dollar VISA 4817 7601 8112 4706

Griggorii@gmail.com
