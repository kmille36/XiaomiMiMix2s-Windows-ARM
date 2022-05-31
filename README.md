Tools link: https://drive.google.com/file/d/1-w8TNVzqBj442bn5MXVjSnlI9wNr_JCc/view?usp=sharing
  - Or download manually: https://renegade-project.org/#/en/windows/Installation-guide

TWRP link: https://twrp.me/xiaomi/xiaomimimix2s.html

SIM Support: https://forum.renegade-project.org/t/mix2s-polaris-qcn/1268
  - adb shell > su > setprop sys.usb.config diag,adb

You need to flash devcfg partition with the provided image. Link: http://files.renegade-project.org/devcfg-polaris_FixTS.img with command: fastboot flash devcfg_ab devcfg-polaris_FixTS.img

WOA Driver for Mi Mix 2S: https://github.com/edk2-porting/WOA-Drivers/releases/download/v1.1.1/polaris.tar.gz

Windows 11 Dev ISO link (recommend): https://drive.google.com/file/d/1qnuMruzqVTvsahVQMe7F4b4IbhsUzr6-/view?usp=sharing

Windows 10 Pro ISO link (x64 app not supported): https://drive.google.com/file/d/1iile3xCUhLHxjzJEBj843ViUPLA6UfRx/view?usp=sharing

HDMI via DisplayLink: USB 3.0 to HDMI Ugreen 40229

![z3319353158028_ddf749c2cb8430116faacc23dcb64e5c](https://user-images.githubusercontent.com/58414694/161889855-d5792d90-c82b-47ff-8fc2-0891e41faf74.jpg)

![image](https://user-images.githubusercontent.com/58414694/155492248-047e4360-e764-45c5-a0fe-959516f26fd2.png)

![image](https://user-images.githubusercontent.com/58414694/154401085-158931b3-8fd5-4adc-9786-ca7a82b5f793.png)

![image](https://user-images.githubusercontent.com/58414694/154398603-d881e278-1df9-4203-845d-a85b9fd4fd0e.png)

![image](https://user-images.githubusercontent.com/58414694/154398734-c84fb992-eca5-4d0d-97ee-db81c945a102.png)

![image](https://user-images.githubusercontent.com/58414694/154399964-8c23c776-51dc-4900-9ecc-5168b2844784.png)

![image](https://user-images.githubusercontent.com/58414694/154399776-6790111e-3646-4e25-9ddb-2e1ad2975feb.png)

* Delete Windows ARM? Do parted step same as install, then rm esp, pe, win, userdata (rm 21, rm 22, rm 23, rm24) and make new userdata with command: 

![image](https://user-images.githubusercontent.com/58414694/171090939-eaeba3e7-c753-4867-9664-b927091cbf91.png)

 + mkpart userdata ext4 1611MB 59.1GB (64GB model)
 + mkpart userdata ext4 1611MB 123GB (128GB model)
 + mkpart userdata ext4 1611MB 253GB (256GB model)
