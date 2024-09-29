These two files are applicable for proot-distro on Termux (Android 5.0-7.0). Follow the steps below to manually install them on the older Termux version:

Reference Article: Using Termux on Android to Create Your Linux Terminal

If your system is Android 7.0 or above, you can use the method described in the article.

For Android 5.0-7.0, you must use the following approach.

Source: Downloaded from my GitHub, based on the latest Termux version.

Download the Files
First, download the following files to your Termux environment:
```
wget https://github.com/TokiZeng/proot-distro-for-Termux-Android-5.0-7.0/blob/main/proot-distro_4.16.0_all.deb
```
```
wget https://github.com/TokiZeng/proot-distro-for-Termux-Android-5.0-7.0/blob/main/proot_5.1.107-65_aarch64.deb
```
Install proot
Run the following command to install proot:

apt install ./proot_5.1.107-65_aarch64.deb

This will install an updated version of proot, solving compatibility issues.

Install proot-distro
Next, run the command below to install proot-distro:

apt install ./proot-distro_4.16.0_all.deb

This will install proot-distro, allowing you to install and manage various Linux distributions in Termux.

Verify Everything is Working
After the installation is complete, run the following command to confirm that proot-distro is functioning correctly:

proot-distro list

And that's it! You can now successfully use proot-distro on Termux for Android 5.0-7.0!
