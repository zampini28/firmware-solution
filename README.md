# firmware-solution
debian 11 graphical installation problem how to provide non-free firmware files missing iwlwifi-6000g2a-5.ucode and iwlwifi-6000g2a-6.ucode.

First, download iwlwifi-6000g2a-5.ucode and iwlwifi-6000g2a-6.ucode files from this repository. 
You can also see all the files in https://github.com/OpenELEC/iwlwifi-firmware.

Use the command prompt to cd to the USB stick  – be sure that you're in the right directory.

Then, write and execute the following code in the command prompt 

```
mkdir /lib/firmware
mount /dev/sdc1 /lib/firmware
```

Finally, try again the installation with F9 to deboot opitions. The installation should go flawlessly.	
