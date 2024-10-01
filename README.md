These two files are applicable for proot-distro on Termux (Android 5.0-7.0). Follow the steps below to manually install them on the older Termux version:

Reference Article: [Using Termux on Android to Create Your Linux Terminal](https://lyingflat.info/2024/09/29/%e5%9c%a8-termux-%e4%b8%ad%e4%bd%bf%e7%94%a8-ssh-%e9%80%a3%e6%8e%a5%e4%b8%a6%e5%ae%89%e8%a3%9d-ubuntu%ef%bc%9a%e5%ae%8c%e6%95%b4%e6%95%99%e5%ad%b8/)

For Android 5.0-7.0 (arm64-v8a), you must use the following approach.

Download the Files
First, download the following files to your Termux environment:
```
curl -L -o proot-distro_4.16.0_all.zip https://github.com/TokiZeng/proot-distro-for-Termux-Android-5.0-7.0/raw/main/proot-distro_4.16.0_all.zip
```

```
unzip proot-distro_4.16.0_all.zip
```

Install proot
Run the following command to install proot:
```
apt install ./proot_5.1.107-65_aarch64.deb
```
This will install an updated version of proot, solving compatibility issues.

Install proot-distro
Next, run the command below to install proot-distro:
```
apt install ./proot-distro_4.16.0_all.deb
```
This will install proot-distro, allowing you to install and manage various Linux distributions in Termux.

Verify Everything is Working
After the installation is complete, run the following command to confirm that proot-distro is functioning correctly:
```
proot-distro list
```
And that's it! You can now successfully use proot-distro on Termux for Android 5.0-7.0!
