# my way to chroot my Enterprise Linux 

1. Insert a bootable media which contains a dvd-iso of installed distro  
   in my case Rocky linux  
2. Boot from bootable media 
3. Select Troubleshoot ( it will actually work not like microsoft's )
4. Select Rescue ${distro name of dvd-iso}
5. Skip to Shell
6. <pre> # lsblk  </pre>
7. <pre > #  mount   /dev/nvme01p1    /mnt </pre>
8. <pre> # cd   /mnt </pre> 
9. <pre> # ls </pre> 
10.<pre> # chroot  /mnt  </pre>
11. \# ls 
12. now you are in your currupted os's fs.

### now you can modify your currupted os and repair it if you know what is the cause of problem.

