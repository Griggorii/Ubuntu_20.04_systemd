# ubuntu_20.04_systemd
ubuntu , zfs , systemd , fb , 20.04

Check /usr/lib/x86_64-linux-gnu/libc-2.31.so 

Ubuntu 20.04 

Deb package https://github.com/Griggorii/Ubuntu_20.04_systemd/releases/tag/systemd_245.4-4ubuntu3.11

Development dev https://github.com/Griggorii/busybox-1.33.0-ubuntu-20.04 inpack busybox-1.33.0_full_add_library_functions.tar.xz find test $ sudo cp test /usr/bin/

$ ./systemd-service-fstrim-on-upgrade-check-off

Reconfigure gdm3/lightdm/sddm just in case choose your option | на всякий случай выберите ваш вариант и пере деконфигурируйте

$ sudo dpkg-reconfigure gdm3

$ sudo dpkg-reconfigure lightdm

$ sudo dpkg-reconfigure sddm

Reboot

OS https://youtu.be/MVhZ_QZGxaQ

______________________________________________________________________________________________________________________________________________

                       Griggorii@gmail.com выключение некоторых пока лишних сервисов сработает после перезагрузки
                                       
                       Griggorii@gmail.com turning off some of the unnecessary services will work after reboot

RUS: Внимание ! всю информацию которую вы списываете относится к исследованиям griggorii как к авторскому праву и документу любое перекопирование с указанием ссылки на исследования от griggorii

Eng: Attention ! all information that you write off refers to the research of griggorii as a copyright and document any copying with a link to the research from griggorii

/etc/systemd/system

# OFF superfluous | выключение лишних сервисов

sudo systemctl disable cron

sudo systemctl disable libvirt-guests

sudo systemctl disable libvirtd

sudo systemctl disable rsync

sudo systemctl disable avahi-daemon

sudo systemctl disable binfmt-support

sudo systemctl disable cups-browsed | осторожно относится к принтеру если нету принтера

sudo systemctl disable cups | осторожно относится к принтеру если нету принтера

sudo systemctl disable secureboot-db

sudo systemctl disable remote-fs

sudo systemctl disable machines

sudo systemctl disable qemu-kvm

sudo systemctl disable anacron

sudo systemctl disable gpu-manager

sudo systemctl disable sshd

sudo systemctl disable ssh

sudo systemctl disable ssh2

sudo systemctl disable lm_sensors

# On superfluous | включение сервисов

sudo systemctl enable cron

sudo systemctl enable libvirt-guests

sudo systemctl enable libvirtd

sudo systemctl enable rsync

sudo systemctl enable avahi-daemon

sudo systemctl enable binfmt-support

sudo systemctl enable cups-browsed

sudo systemctl enable cups

sudo systemctl enable secureboot-db

sudo systemctl enable remote-fs

sudo systemctl enable machines

sudo systemctl enable qemu-kvm

sudo systemctl enable anacron

sudo systemctl enable gpu-manager

sudo systemctl enable sshd

sudo systemctl enable ssh

sudo systemctl enable ssh2

sudo systemctl enable lm_sensors

# Danger ! OFF internet systemd reboot

sudo systemctl disable systemd-resolved

# ON internet systemd reboot

sudo systemctl enable systemd-resolved

______________________________________________________________________________________________________________________________________________


New glibc wayland not freeze https://github.com/Griggorii/glibc-2.31_all.deb_package_version_libc6-prof_2.31-0ubuntu9.2_amd64.deb_ubuntu_20.04_focal_fossa

Only real technologies, not any fictional parasitic distributions support real technology investments and donate dollar VISA 4817 7601 8112 4706

Griggorii@gmail.com
