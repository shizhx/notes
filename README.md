# 备忘录
记录工作或生活中的点滴技巧

## Ubuntu 禁用笔记本触摸板
```shell
➜  ~ xinput list # 列出所有输入设备
⎡ Virtual core pointer                    	id=2	[master pointer  (3)]
⎜   ↳ Virtual core XTEST pointer              	id=4	[slave  pointer  (2)]
⎜   ↳ Holtek USB Gaming Mouse                 	id=13	[slave  pointer  (2)]
⎜   ↳ FSPPS/2 Sentelic FingerSensingPad       	id=15	[slave  pointer  (2)]
⎣ Virtual core keyboard                   	id=3	[master keyboard (2)]
    ↳ Virtual core XTEST keyboard             	id=5	[slave  keyboard (3)]
    ↳ Power Button                            	id=6	[slave  keyboard (3)]
    ↳ Video Bus                               	id=7	[slave  keyboard (3)]
    ↳ Video Bus                               	id=8	[slave  keyboard (3)]
    ↳ Power Button                            	id=9	[slave  keyboard (3)]
    ↳ Sleep Button                            	id=10	[slave  keyboard (3)]
    ↳ USB Webcam                              	id=11	[slave  keyboard (3)]
    ↳ Holtek USB Gaming Mouse                 	id=12	[slave  keyboard (3)]
    ↳ AT Translated Set 2 keyboard            	id=14	[slave  keyboard (3)]

➜  ~ xinput set-prop 15 "Device Enabled" 0 # 禁用触摸板
```
