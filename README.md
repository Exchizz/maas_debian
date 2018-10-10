# maas_debian
curtin config to deploy debian using Ubuntu Maas


Follow https://askubuntu.com/a/973247/872443 to upload debian-cloud-image to ubuntu maas.


Partition layout will be as shown below:
NAME                MAJ:MIN RM   SIZE RO TYPE MOUNTPOINT
sda                   8:0    0 111.8G  0 disk 
├─sda1                8:1    0  1004K  0 part 
├─sda2                8:2    0     1G  0 part /boot
├─sda3                8:3    0    24G  0 part 
└─sda4                8:4    0  86.8G  0 part 
  ├─VolGroup01-root 254:0    0     5G  0 lvm  /
  ├─VolGroup01-usr  254:1    0     5G  0 lvm  
  └─VolGroup01-var  254:2    0     5G  0 lvm  
sdb                   8:16   0   9.1T  0 disk 
