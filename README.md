SETUP#1 macbookpro - MacOS dual boot + BACKUP drive
MacOS for High Sierra + Ventura

1.PNY sda 1TB (caddy) - |High Sierra - 250GB| + |BACKUP(ext2) - 750GB| 

2.PNY sdb 500GB - |Ventura + OCLP(open-core legacy patcher)

Order of instalation
1. sda1 High Sierra
2. sda2 BACKUP Drive
3. sdb - Open-Core Legacy Patcher to sb1
4. sdb1 - Ventura
   

============================================================================


SETUP#2 macbookpro - Triple Boot - Windows - Kali - Parrot + SHARED

1.#PNY sdb 931.51 GB (caddy) - |Windows- 240310 MB| + |Parrot - 691200 MB| 

2.#ADATA sda 953.86 GB - |Kali - 701620 MB| + |Shared - 252240 MB| + 

Order of Installation
1. install sdb alone (PNY) (240310 mb) - Windows
2. allocate/format sb2 (691200) to EXT2 - Parrot
3. Install sdb (ADATA)  
4. allocate/format sda1 (716800 mb) - Kali (Format EXT2)
5. allocate/format sda2 (252240 mb) - SHARED (Format NTFS)
6. delete sda1 volume Kali
7. install Kali using sda1 (716800 mb) - largest free space
8. delelet sb2 volume (691200 mb) - Parrot
9. install Parrot on sdb (691200 mb free space), replace a partition (use free space) & EFI system partition (Kali) /dev/sda3
10. install rEFInd (disables secure boot which is requirement to fix windows audio issue)
11. re-install rEFInd to fix Grub issue and create triple boot option
12. hide un-needed options
13. install/fix windows audio issues
14. Run batman.sh on Kali and parrot.sh on Parrot
15. Configure GRUB of Kali and Parrot
16. Configure the things to do after installing Kali
