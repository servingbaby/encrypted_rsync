# encrypted_rsync
Rsync to LUKS


Used the following resources:
blog.farville.com/automated-encrypted-backups-with-rsync-and-dm-crypt/
www.cyberciti.biz/hardware/howto-linux-hard-disk-encryption-with-luks-cryptsetup-command/
======================================================
$ cryptsetup luksOpen /dev/xvdc encrypted
$ mount /dev/mapper/encrypted /mnt/encrypted/
$ umount /mnt/encrypted/
$ cryptsetup luksClose encrypted
========================================================

