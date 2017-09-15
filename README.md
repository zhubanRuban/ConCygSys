# ConCygSys
![ConCygSys](https://github.com/zhubanRuban/cygwin-extras/raw/master/img/concygsys.png)

**ConEmu / CygWin Portable for SysAdmins**

-------------------

This is an independent fork of amazing [cygwin-portable-installer](https://github.com/vegardit/cygwin-portable-installer) project

**Modded specially for sysadmin purposes. Your Linux shell On Windows**

This will install portable [CygWin](https://www.cygwin.com/) environment and connect to portable [ConEmu](https://conemu.github.io/) console emulator, so you will have all required tools for server management in one folder which can be moved between PCs and/or run from USB stick

--------------------

## Installation

- create a folder on your PC where you want to store ConCygSys, let it be `D:\concygsys\`
- download installer from [this link](https://github.com/zhubanRuban/ConCygSys/archive/master.zip) (right click > save link as) to `D:\concygsys\`
- launch `ConCygSys-installer.cmd` you downloaded to `D:\concygsys\`
- once the installation is finished, launch the desired shell:
  `ConCygSys.cmd` to run CygWin via ConEmu (if chosen to install) - recommended and the most convenient option
  `ConCygSys-bash.cmd` to run CygWin in standard Windows console
  `ConCygSys-bash.cmd` to run CygWin via [MinTTY](https://mintty.github.io/) terminal emulator (if chosen to install)
- have fun

## Customization

If you open `ConCygSys-installer.cmd` with [Notepad++](https://notepad-plus-plus.org/) (forget about standard Notepad, it will mess everything up), you will get a control over the installation settings.

**Available options:**

- `CYGWIN_USERNAME` - the desired username (defaults to root)
- `CYGWIN_MIRROR` - the source you would like to download CygWin from - [full list of available mirrors](https://cygwin.com/mirrors.html)
- `CYGWIN_PACKAGES` - packages to install - [full list of availbale packages](https://cygwin.com/packages/package_list.html)
- `INSTALL_APT_CYG` - install [apt-cyg package manager](https://github.com/transcode-open/apt-cyg) alows to install/remove [packages](https://cygwin.com/packages/package_list.html) from command line
- `INSTALL_BASH_FUNK` - install [bash-funk - adaptive Bash prompt](https://github.com/vegardit/bash-funk)
- `INSTALL_PSSH` - install [Parallel SSH tool on bash](https://github.com/zhubanRuban/cygwin-extras#pssh-parallelssh)
- `INSTALL_PSCP` - install [Parallel SCP tool on bash](https://github.com/zhubanRuban/cygwin-extras#pscp-parallelscp)
- `INSTALL_SSH_AGENT_TWEAK` - install [SSH agent enhancements](https://github.com/zhubanRuban/cygwin-extras#re-use-ssh-agent)
- `INSTALL_BASHRC_CUSTOMS` - install [Bash prompt enhancements](https://github.com/zhubanRuban/cygwin-extras#custom-bashrc) (disables bash-funk)

## Important Note

In order to install ConCygSys successully, make sure you uninstalled any existing non-portable [CygWin](https://cygwin.com/faq/faq.html#faq.setup.uninstall-all) and [ConEmu](https://conemu.github.io/en/Installation.html) instances.

## License

All files are released under the [Apache License 2.0](https://github.com/vegardit/bash-funk/blob/master/LICENSE.txt).

## Where can I report an issue?

[Here](https://github.com/zhubanRuban/ConCygSys/issues)
