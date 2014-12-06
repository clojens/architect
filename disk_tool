#!/usr/bin/env zsh


#
# My personal schema
#
# 01 bios boot partition        +2M ef02
# 02 swap partition             RAM * 2 (keep at beginning or end for less spinning if magentic disk)
# 03 os boot partition          < 700M (more than enough even with a couple of kernels installed)
# 04 root partition             < 10G (way way enough for only /root and /etc basically)
# 05 usr static program files   ~ 25G (and that might still be a bit too small, depends on disk size)
# 06 usr local super-user own   ~ 10G (for software that might had gone /opt or even /home/user we can own + save here)
# 07 variable data              < 18G (should be well enough, else clean pacman cache and clean logs)
# 08 external services          < 20G (web hosted files and services should be enough but tweakable)
# 09 optional standalone apps   > 10G (can be anything really, if not headless, e.g. chrome will take space)
# 10 user data home files       > 10G (can be anything really)
# 11 temporary files            rest  (not for actual storage as we use tmpfs but jails etc)














#target_disk=/dev/sda
#
#diskspace=$(( $(grep ${target_disk##*/}$ /proc/partitions | awk '{print $3}') * 2 / 2048 - 1 ))
#swapspace=$(( $(head -n1 /proc/meminfo | awk '{print $2}') / 1024 + 1 ))
#rootspace=$(( $diskspace - $swapspace ))
#
#sgdisk --clear --new 1:0:+${rootspace}MiB --new 2:0:+${swapspace}MiB --typecode 2:8200 ${dry_run:-'--pretend'} --print $target_disk



