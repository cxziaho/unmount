# unmount by cxziaho
Unmount and Remount all drives from PS Vita  
Enables RW access just like [VitaRW](https://github.com/tomtomdu80/VitaRW) by `Major_Tom` does, but in a kernel plugin, on boot.  
Fixes the sa0 and pd0 unmount problems.  
There are builds for this one though o_0 - **BE CAREFUL**.
  
----
  
## Install
Move unmount.skprx to `ur0:tai/` and add to your `config.txt`:
```
*KERNEL
ur0:tai/unmount.skprx
```  
  
## Building   
Assuming you have the [VitaSDK](http://vitasdk.org) toolchain:  
```  
git clone https://github.com/cxziaho/unmount.git  
cd unmount  
cmake .  
make  
```  
and use unmount.skprx  
  
## Uninstall
Remove unmount.skprx from `config.txt` and `ur0:tai/`, then restart your Vita.