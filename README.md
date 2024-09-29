proot-distro for Termux on Android 5.0-7.0
These two files are compatible with proot-distro for Termux (Android 5.0-7.0) and can be manually installed on the older Termux version through the following steps:

Source: My GitHub, extracted from the latest version of Termux.

1. Download the Files
First, download both files into your Termux environment:

bash
wget https://github.com/TokiZeng/proot-distro-for-Termux-Android-5.0-7.0/blob/main/proot-distro_4.16.0_all.deb
wget https://github.com/TokiZeng/proot-distro-for-Termux-Android-5.0-7.0/blob/main/proot_5.1.107-65_aarch64.deb
2. Install proot
Run the following command to install proot:

bash
apt install ./proot_5.1.107-65_aarch64.deb
This will install the updated version of proot to resolve compatibility issues.

3. Install proot-distro
Next, install proot-distro using the command below:

bash
apt install ./proot-distro_4.16.0_all.deb
This will install proot-distro and allow you to install and manage various Linux distributions within Termux.

4. Verify the Installation
After installation, you can check if proot-distro is working properly by running:

bash
proot-distro list
And that’s it! You can now successfully use proot-distro within Termux on Android 5.0-7.0!
