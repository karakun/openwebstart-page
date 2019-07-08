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

<span class="my-karakun">Open</span>WebStart 0.2.0 comes with a user-friendly installer. Download the "stable" build to try out the <span class="text-highlight">Open<span>WebStart</span></span> alpha release now!

## How to Install <span class="my-karakun">Open</span>WebStart on Microsoft Windows

1. Go to the [download area](/download) and download `OpenWebStart_windows-x64_0_2_x-alpha.zip`.
1. Run the installer.
1. Choose a language and click **OK** to open the <span class="my-karakun">Open</span>WebStart Setup wizard. 
1. Click **Next** to start the <span class="my-karakun">Open</span>WebStart installation.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click **Next**. 
   <br />Windows default: `C:\Program Files\OpenWebStart`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click **Next**.
1. Wait while Setup installs <span class="my-karakun">Open</span>WebStart on your computer.
1. Click **Finish** on the completion screen to close the wizard.

## How to Install <span class="my-karakun">Open</span>WebStart on Linux

1. Go to the [download area](/download) and download the linux installer:
   * For Debian Linux, download `OpenWebStart_linux_2_0.deb`
   * For other Linux distributions, download `OpenWebStart_linux_2_0.sh`
1. Change into the installer directory and run the installer from the terminal: 
   * For Debian Linux: `sudo dpkg -i OpenWebStart_linux_0_2.deb`
   * For other Linux distributions: `sudo chmod u+x ./OpenWebStart_linux_2_0.sh; sudo ./OpenWebStart_linux_0_2.sh`
1. Enter your root password.
1. Choose a language and click **OK** to open the <span class="my-karakun">Open</span>WebStart Setup wizard. 
1. Click **Next** to start the <span class="my-karakun">Open</span>WebStart installation.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click **Next**. 
   <br />Default: `/opt/openwebstart`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click **Next**.
1. Please wait for <span class="my-karakun">Open</span>WebStart to be installed on your computer.
1. Click **Finish** on the completion screen to close the wizard.

## How to Install <span class="my-karakun">Open</span>WebStart on macOS

1. Go to the [download area](/download) and download `OpenWebStart_macos_0_2_x-alpha.dmg`.
1. Open the OpenWebStart disk image to mount it. 
1. Run the installer app.
   <br />Note: If you get a message that this app is from an unidentified developer, click **OK**.
   1. Choose **Apple menu > System Preferences**, click **Security & Privacy**, and go to the **General** tab. 
   1. Click the lock and enter your password.
   1. Click “Open Anyway” to allow the <span class="my-karakun">Open</span>WebStart installer to run. 
1. Choose a language and click **OK** to open the <span class="my-karakun">Open</span>WebStart Setup wizard. 
1. Click **Next** to start the <span class="my-karakun">Open</span>WebStart installation.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click **Next**. 
   <br />Default: `/Applications/Open Web Start`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click **Next**.
1. Please wait for <span class="my-karakun">Open</span>WebStart to be installed on your computer.
1. Click **Finish** on the completion screen to close the wizard.

# How to Use <span class="my-karakun">Open</span>WebStart

<span class="my-karakun">Open</span>WebStart installs an executable called `javaws` that can run Java Web Start apps (.JNLP suffix). During the development phase, the <span class="my-karakun">Open</span>WebStart installer will not change file associations of any existing Oracle `javaws` executable, so you can use both.

To run .JNLP applications with `javaws` from the command line or terminal:
  * Windows Command Line example:
  <br />`C:\Program Files\OpenWebStart\javaws -nosecurity -Xnofork -jnlp myApp.jnlp -console`
  * macOS/Linux Terminal example:
  <br /> `/Applications/Open Web Start/javaws -nosecurity -Xnofork -jnlp myApp.jnlp -console`

To run .JNLP applications with <span class="my-karakun">Open</span>WebStart from Windows Explorer:

1. Right-click the JNLP app and select **Open With -&gt; Choose Another App**.
1. Click **More Apps** and scroll down.
1. Click **Look for Another App on this PC**.
1. Browse to <span class="my-karakun">Open</span>WebStart at `C:\Program Files\OpenWebStart\javaws`.
1. Click **Open** to associate this JNLP file with <span class="my-karakun">Open</span>WebStart.

To run .JNLP applications with <span class="my-karakun">Open</span>WebStart from the macOS Finder:

1. Right-click the JNLP app and select **Open With -&gt; Other...**.
1. Browse to <span class="my-karakun">Open</span>WebStart at `/Applications/Open Web Start/javaws`.
1. Click **Open** to associate this JNLP file with <span class="my-karakun">Open</span>WebStart.

## How to perform an unattended installation

1. Install <span class="my-karakun">Open</span>WebStart for your operating system as described in this article.
   <br />The installer creates a response file that stores the options that you have chosen in the installer.
1. Run the installer again from the command line with the parameter ` -q -varfile response.varfile` to execute an unattended installation.
   * For Windows: `OpenWebStart_windows_Setup.exe -q -varfile response.varfile`
   * For macOS: `OpenWebStart_macos_0_2_x-alpha.dmg -q -varfile response.varfile`
   * For Debian Linux: `sudo OpenWebStart_linux_2_0.deb -q -varfile response.varfile`
   * For other Linux distributions: `sudo ./OpenWebStart_linux_1_0.sh -q -varfile response.varfile`

For more information, see https://www.ej-technologies.com/resources/install4j/help/doc/index.html#install4j.installers.installerModes .

# How to Uninstall <span class="my-karakun">Open</span>WebStart

1. Go to your <span class="my-karakun">Open</span>WebStart directory. 
1. Run the Uninstaller.
1. Click **Next** in the <span class="my-karakun">Open</span>WebStart Uninstaller wizard.
1. Wait for the Uninstaller to complete.
1. Click **Finish** on the completion screen to close the wizard.
