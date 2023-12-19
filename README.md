# MSI B660M-E DDR4 i5-12400F RX 590 GME Hackintosh EFI

------



配了一台组装机，12代i5加AMD独显，这配置，本以为轻松黑苹果，结果遇到点障碍，就把折腾过程记录下来。

## 0.经验教训

首先，显卡RX 590 GME，这个是不被MacOS支持的，必须刷显卡BIOS刷成580，可参考[刷显卡过程](./VBIOS/README.md)。另外，网上还有说不刷VBIOS，通过仿冒显卡ID的方式，但是我没有成功。

另外，按照网上的教程，自己配了opencore的EFI，但是无论怎么折腾，都报错。GitHub上找到了别人的MSI B660M的EFI（不是B660M-E是其他型号），一样报错。后来上网买了别人做好的MSI B660M-E DDR4主板加i5 12400的EFI，还是一样的报错。

一度怀疑运气不好，电脑就是不支持MacOS，直到看到了大神的[这篇帖子](https://www.olarila.com/topic/5676-hackintosh-efi-folder-with-clover-and-opencore/)，试了一下，终于成功了。里面给出了[12代CPU](./EFI/EFI.Opencore.Desktop.AlderLake.zip)和[13代CPU](./EFI/EFI.Opencore.Desktop.RaptorLake.zip)的通用的EFI，我下载了12代的EFI，修改了一下，成功了。

这里得到的经验就是，只要报错，直接换EFI。



1.配置



BIOS设置



