# To open an encrypted partition /dev/sdb1 (reachable at /dev/mapper/backup):

cryptsetup open --type luks /dev/sdb1 backup

# To open an encrypted partition /dev/sdb1 using a keyfile (reachable at /dev/mapper/hdd):

cryptsetup open --type luks --key-file hdd.key /dev/sdb1 hdd

# To close luks container at /dev/mapper/hdd:

cryptsetup close hdd
