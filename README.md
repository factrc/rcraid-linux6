# rcraid-linux6
Inofficial patch driver AMD RAID( aka rcraid ) to work in linux 6.3 and above

# patch-linux6-810 
Applying the patches is done by hand. I use the rcraid-dkms package from [Thomas Karl Pietrowski (@thopiekar). ](https://github.com/thopiekar/rcraid-dkms)   
Testing Fedora 38 with kernel 6.3.12-200 and 6.4.4-200.

`Support only AM4(AM5) chipset`


# patch-linux6-930
Applying the patches is done by hand. I use official driver AMD for Linux by link: [Official driver](https://www.amd.com/en/support/chipsets/amd-socket-strx4/trx40)   
Testing Fedora 38 with kernel 6.3.12-200 and 6.4.4-200.   
`Support TRX40 chipset & raid5 & NVME, and only legacy type for AM4.`


# Instruction 
Download the driver from the link above. 

`cd <driver_path>`    
`patch -p1 <patch-linux6-810`   
`Follow the instructions in the driver.`   

or

`cd <driver_path>/driver_sdk`   
`patch -p1 <patch-linux6-930`   
`Follow the instructions in the driver.`   

Free code driver it's same ( little difference ), but blob other.    
I not include patch in blob for working 930 in AM4.   
