SETUP#1 macbookpro - MacOS dual boot + BACKUP drive
MacOS for High Sierra + Ventura
PNY sda 1TB (caddy) - |High Sierra - 250GB| + |BACKUP(ext2) - 750GB| 
PNY sdb 500GB - |Ventura + OCLP(open-core legacy patcher)
Orfer of instalation
1. sda1 High Sierra
2. sda2 BACKUP Drive
3. sdb - Open-Core Legacy Patcher
4. sdb1 - Ventura 


SETUP#2 macbookpro - Triple Boot - Windows - Kali - Parrot + SHARED
PNY sda 931.51 GB (caddy) - |Windows - 245760 MB| + |Parrot - 680960 MB |
ADATA sdb 953.86 GB - |Kali - 667702 MB| + |Shared - 286158 MB|
Order of Installation
1. sda1 - Windows
2. sb1 - Kali
3. sb2 - SHARED
4. install rEFInd (disables secure bootwhich is requirement to fix windows audio issue)
5. install/fix windows audio issues
6. sd2 - Parrot (EFI system partition: /dev/sb3)
7.  
