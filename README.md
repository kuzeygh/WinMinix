# A MINIX environment for Windows based on QEMU.

MINIX 3 is a UNIX-like operating system created with the goal of being a highly reliable and self-healing microkernel OS. MINIX 3 includes ssh, emacs, vi, perl, python, bash, X11, ftp, pine, clang, and gcc tools. Updated binary and source packages are available for MINIX 3. MINIX 3 is available under a BSD license and supports many programming languages and development tools.

**Installation steps:**
* Download and unzip [zip](https://github.com/sirredbeard/WinMinix/archive/master.zip) of this git repo.
* Run GetMINIX.bat to download MINIX iso.
* Run InstallMINIX.bat install MINIX to built-in virtual hard-drive
    * Select option 1 in the boot menu
    * Login as 'root', no password required
    * Type setup at the shell
    * Follow the prompts and you can usually accept all defaults unless you have made specific customizations
    * Back at shell, type shutdown -h now, and close window when indicates it is safe to do so.
* Run WinMINIX.bat to boot freshly installed MINIX.
    * Use WinMinix-X11.bat with settings optimized for X11, but creates an additional window.
    * Use WinMinix-sshd.bat to launch a headless MINIX instance ssh pass-through via localhost:2200. Note: sshd must be properly configured on MINIX first. See [sshd documentation](https://wiki.minix3.org/doku.php?id=usersguide:settingupssh).
* Consult [post installation documentation](https://wiki.minix3.org/doku.php?id=usersguide:postinstallation) for MINIX, including installing binary packages using [pkgin](https://wiki.minix3.org/doku.php?id=usersguide:installingbinarypackages) or from source using NetBSD's [pkgsrc](https://wiki.minix3.org/doku.php?id=usersguide:installingsourcepackages) repo.

**Hacking this project:**
* Optimize QEMU for your particular hardware by tweaking command-line settings in WinMINIX.bat.
* Fork this project and replace MINIX with another obscure operating system.
* Add a reliable way to perform SHA1 verification on downloads.

**Made from:**
* [MINIX 3.4.0-rc6](http://download.minix3.org/iso/snapshot/), which has parts from FreeBSD and NetBSD.
* [QEMU 3.0.0-rc1](https://qemu.weilnetz.de/w64/)
* [wget 1.19.4](https://eternallybored.org/misc/wget/)
* [7-zip 18.05](https://www.7-zip.org/)

**Licenses:**
* [QEMU](https://wiki.qemu.org/License) is licensed under the GPL2 license.
* [wget](https://www.gnu.org/software/wget/) is licensed under the GPL3 license.
* [MINIX](https://github.com/minix3/minix/blob/master/LICENSE) is licensed under the BSD license.
* [7-Zip](https://www.7-zip.org/faq.html) is licensed under the LGPL license.
* This project is licensed under the GPL2 license.

Written using Notepad and Visual Studio Code on Windows 10 Pro.

**Other projects:**
* [Awesome UNIX](https://github.com/sirredbeard/Awesome-UNIX)
* [Awesome WSL](https://github.com/sirredbeard/Awesome-WSL)