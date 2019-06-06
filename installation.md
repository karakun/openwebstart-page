---
layout: article
title: Installation
order: '16'
headerText:
permalink: /installation/
header:
  text: How to install <span class="my-karakun">Open</span>WebStart
nav:
  bottom: false
---

# How to install <span class="my-karakun">Open</span>WebStart

<span class="my-karakun">Open</span>WebStart comes with a user-friendly installer for Windows, macOS, and Linux. Choose a "stable" build to try out the <span class="text-highlight">Open<span>WebStart</span></span> alpha release, or choose a nightly build to try out the latest untested features.

## How to Install <span class="my-karakun">Open</span>WebStart on Microsoft Windows

1. Go to https://openwebstart.com/download and download OpenWebStart_windows-x64_1_0-SNAPSHOT.exe.
1. Run the installer.
1. Choose a language and click OK. 
1. In the <span class="my-karakun">Open</span>WebStart Setup Wizard, click Next.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click Next. 
   <br />Default: `C:\Program Files\OpenWebStart`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click Next.
1. Please wait while Setup installs <span class="my-karakun">Open</span>WebStart on your computer.
1. Click Finish on the completion screen to close the wizard.

## How to Install <span class="my-karakun">Open</span>WebStart on macOS

1. Go to https://openwebstart.com/download and download OpenWebStart_macos_1_0.dmg.
1. Open the OpenWebStart disk image to mount it. 
1. Run the installer app.
    <br />Note: If you get a message that this app is from an unidentified developer, click OK.
    1. Choose Apple menu > System Preferences > Security & Privacy, and go to the General tab. 
    1. Click the lock and enter your password.
    1. Click “Open Anyway” to allow the <span class="my-karakun">Open</span>WebStart installer to run. 
1. Choose a language and click OK. 
1. In the <span class="my-karakun">Open</span>WebStart Setup Wizard, click Next.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click Next. 
    <br />Default: `/Applications/Open Web Start`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click Next.
1. Please wait while Setup installs <span class="my-karakun">Open</span>WebStart on your computer.
1. Click Finish on the completion screen to close the wizard.

## How to Install <span class="my-karakun">Open</span>WebStart on Linux

1. Go to https://openwebstart.com/download and download the linux installer:
   * For Debian Linux, download OpenWebStart_linux_1_0-SNAPSHOT.deb
   * For other Linux distributions, download OpenWebStart_linux_1_0-SNAPSHOT.sh
1. Run the installer from the terminal: 
   * For Debian: `sudo dpkg -i OpenWebStart_linux_1_0.deb`
   * For others: `sudo chmod u+x ./OpenWebStart_linux_1_0.sh; sudo ./OpenWebStart_linux_1_0.sh`
1. Enter your root password.
1. Select a language and click OK. 
1. In the <span class="my-karakun">Open</span>WebStart Setup Wizard, click Next.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click Next. 
   <br />Default: `/opt/openwebstart`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click Next.
1. Please wait while Setup installs <span class="my-karakun">Open</span>WebStart on your computer.
1. Click Finish on the completion screen to close the wizard.

# How to Use <span class="my-karakun">Open</span>WebStart

<span class="my-karakun">Open</span>WebStart installs an executable called `javaws`. Open the terminal and use `javaws` to run your existing Java Web Start applications (.jnlp file suffix).

* Windows:
  `C:\Program Files\OpenWebStart\javaws myApp.jnlp`
* macOS: 
  `/Applications/Open Web Start/javaws myApp.jnlp`
* Linux: 
  `/opt/openwebstart/javaws myApp.jnlp`

During the development phase, the <span class="my-karakun">Open</span>WebStart installer will not change your existing Oracle `javaws` executable, so you can use both.

# How to Uninstall <span class="my-karakun">Open</span>WebStart

1. Go to your <span class="my-karakun">Open</span>WebStart directory. 
   macOS default directory: `/Applications/Open Web Start`
   Windows default directory: `C:\Program Files\OpenWebStart`
   Linux default directory:  `/opt/openwebstart`
1. Run the Uninstaller.
1. In the <span class="my-karakun">Open</span>WebStart Uninstaller Wizard, click Next.
1. Please wait for the Uninstaller to complete.
1. Click Finish on the completion screen to close the wizard.
