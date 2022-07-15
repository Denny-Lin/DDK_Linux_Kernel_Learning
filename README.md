# DDK_Linux_Kernel_Learning
Choose the long term support (LTS) version on an Android device.

# Prerequisites
1. Read https://www.kernel.org/doc/html/latest/process/howto.html#process-howto. </br>
2. Read https://www.linuxfromscratch.org/lfs/read.html. </br>

# GKI
... </br>
## GKI 1.0
We know Android 11 had different kernel versions, e.g., android-4.9-q, ..., android-4.19-stable and android11-5.4. </br>
However, since android11-5.4, Google has started using the generic kernel image 1.0 (GKI 1.0). </br>
It means Android 11, 12, 13 and later devices with kernel 5.4 use GKI 1.0. </br>

## GKI 2.0
On Android 12, 13 and later devices with kernel 5.10, Google uses GKI 2.0. </br>

# Let us get started
I chose android13-5.10. </br> 
For other kernel versions (branches), please refer to https://android.googlesource.com/kernel/manifest/+refs. </br> 
So first, download it by the following commands.

```sh
mkdir android-kernel && cd android-kernel
repo init -u https://android.googlesource.com/kernel/manifest -b common-android13-5.10-lts
repo sync
```

# References
1. https://www.kernel.org/
2. https://source.android.com/devices/architecture/kernel/android-common
3. https://source.android.com/devices/architecture/kernel/generic-kernel-image
4. https://0xax.gitbooks.io/linux-insides/content/
5. https://elixir.bootlin.com/linux/latest/source
6. https://bugzilla.kernel.org/
