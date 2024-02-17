SETUP#1 macbookpro - MacOS dual boot + BACKUP drive
MacOS for High Sierra + Ventura
PNY sda 1TB (caddy) - |High Sierra - 250GB| + |BACKUP(ext2) - 750GB| 
PNY sdb 500GB - |Ventura + OCLP(open-core legacy patcher)
Orfer of instalation
1. sda1 High Sierra
2. sda2 BACKUP Drive
3. sdb - Open-Core Legacy Patcher to sb1
4. sdb1 - Ventura 


SETUP#2 macbookpro - Triple Boot - Windows - Kali - Parrot + SHARED
ADATA sda 953.86 GB - |Windows - 272900 MB| + |Parrot - 680960 MB| 
PNY sdb 931.51 GB (caddy) - |Kali - 680960 MB| + |Shared - 248550 MB| +
Order of Installation
1. sda1 (272900 mb) - Windows
2. sdb1 (680960 mb) - Kali
3. sdb2 (248550 mb) - SHARED (NTFS)
4. install rEFInd (disables secure bootwhich is requirement to fix windows audio issue)
5. install/fix windows audio issues
6. sda2 (680 - Parrot (EFI system partition: /dev/sb3)
7.  re-install rEFInd to fix Grub issue and create triple boot option
