# how_to_fix_buffalo_linkstation_xfs_drive
Just a description of how I fixed my corrupt Buffalo Linkstation XFS disk.

My Linkstation failed, probably because of a power failure, and whenever I started it it worked for a few minutes and then went unreachable.

I tried almost every tool on PC and Mac, but it did not work. I could not read the XFS file system. 

### What ultimately fixed it was:
    1. Mounting the NAS disk in Ubuntu running in Virtual Box.
    2. Rebooting the virtual machine with the NAS disk still connected to the virtual machine.
    3. During boot, Ubuntu fixed the borken XFS partition
    4. Then I put the disk back into the Buffalo NAS and it worked. It was also readable with OSX-FUSE using the FUSE-XFS driver.
    5. Then i copied all files from the NAS and when the copying was done, I used a hammer to smash the NAS into pieces.


GLHF to you.
