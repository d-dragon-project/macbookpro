SETUP#1 macbookpro - MacOS dual boot + BACKUP drive
MacOS for High Sierra + Ventura
PNY sda 1TB - |High Sierra - 250GB| + |BACKUP(ext2) - 750GB|
PNY sdb 500GB - |Ventura + OCLP(open-core legacy patcher)
Orfer of instalation
1. sda1 High Sierra
2. sda2 BACKUP Drive
3. sdb - Open-Core Legacy Patcher
4. sdb1 - Ventura 


SETUP#2 macbookpro - Triple Boot - Windows - Kali - Parrot + SHARED
PNY sda 1TB - |Windows - 50% GB| + |Parrot - 614912 MB |
TEAM sdb 1TB - |Kali - 614912 MB| + |SHARED - 441357 MB|
Order of Installation
1. sda1 - Windows
2. sb1 - Kali
3. sb2 - SHARED
4. install rEFInd (disables secure bootwhich is requirement to fix windows audio issue)
5. install/fix windows audio issues
6. sd2 - Parrot (EFI system partition: /dev/sb3)
7.  
