tutorial-tx1
===

# Get Started Guide

- [v] Flash OS on tx1
  - [v] Prerequisite
    - [v] Download NVIDIA Jetpack to a host ubuntu:14.02 machine ov VM
    - [v] Connect power, lan network to tx1.
    - [v] Optional: Connect serial usb from tx1 to host machine for better monitoring
  - [v] If your using VM
    - [v] Network: bridge network to host machine, which is in the same Lan switch with tx1
    - [v] Storage: at least 20g for JetPack installation, temperary system files during flashing
    - [v] Usb: Enable usb 2.0 with virtualbox expension pack. Add the nvidia usb interface to vm.
    - [v] Miscelleous: Disable machine sleep to prevent expected interruption 
  - [v] Enter force recovery mode
    - [v] Connect recovery line (microusb to usb) from tx1 to host machine
    - [v] Turn on tx1 by click power button. 
    - [v] Hold recovery btn and press reset btn more than two seconds and release to enter usb recovery mode
    - [v] On VM, type `lsub` in terminal should show nvidia usb interface. Redo mode swithc steps
  - [v] Install JetPack on host
    - [v] `chmod +x JetPack-*.run`
    - [v] `./JetPack-*.run` should enter GUI guide. Follow the guidance.
    - [v] Make sure to check (install) the flash target os option.
    - [v] Download all the file.
  - [v] Flash target os
    - [v] Choose network configuration. In my case, VM briged to host connect to the same switch with tx1. Option 1
    - [v] Guide program copy file to tx1, install system images, and enable dhcp, ssh connection
    - [v] Optional: Setup wifi, static ip
- [ ] Run gpu computing
  - [ ]

# References

[nvidia tegra guide](https://developer.nvidia.com/embedded/linux-tegra)

[nvidia user guide](http://developer.download.nvidia.com/embedded/jetson/TK1/docs/2_GetStart/Jeston_TK1_User_Guide.pdf)

(http://demotomohiro.github.io/hardware/jetson_tk1/index.html)

(http://www.bojankomazec.com/2017/02/how-to-install-jetpack-on-jetson-tx1.html)


