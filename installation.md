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

<span class="my-karakun">Open</span>WebStart 0.4.0 comes with a user-friendly installer. Download the "stable" build to try out the <span class="text-highlight">Open<span>WebStart</span></span> alpha release now!

<span class="my-karakun">Open</span>WebStart is released under the [GPL mit Classpath Exception](https://github.com/karakun/OpenWebStart/blob/master/LICENSE.md) license.

## How to Install <span class="my-karakun">Open</span>WebStart on Microsoft Windows

1. Go to the [download area](/download) and download `OpenWebStart_windows-x64_0_4_0.zip`.
1. Run the installer.
1. Choose a language and click **OK** to open the <span class="my-karakun">Open</span>WebStart Setup wizard. 
1. Click **Next** to start the <span class="my-karakun">Open</span>WebStart installation.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click **Next**. 
   <br />Windows default: `C:\Program Files\OpenWebStart`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click **Next**.
1. Wait while Setup installs <span class="my-karakun">Open</span>WebStart on your computer.
1. Click **Finish** on the completion screen to close the wizard.

## How to Install <span class="my-karakun">Open</span>WebStart on Linux

1. Go to the [download area](/download) and download `OpenWebStart_linux_0_4_0.deb`.
1. Change into the installer directory and run the installer from the terminal: 
   <br />`sudo dpkg -i OpenWebStart_linux_0_3_x.deb`
1. Enter your root password.
1. Choose a language and click **OK** to open the <span class="my-karakun">Open</span>WebStart Setup wizard. 
1. Click **Next** to start the <span class="my-karakun">Open</span>WebStart installation.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click **Next**. 
   <br />Default: `/opt/openwebstart`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click **Next**.
1. Please wait for <span class="my-karakun">Open</span>WebStart to be installed on your computer.
1. Click **Finish** on the completion screen to close the wizard.

## How to Install <span class="my-karakun">Open</span>WebStart on macOS

1. Go to the [download area](/download) and download `OpenWebStart_macos_0_4_0.dmg`.
1. Open the OpenWebStart disk image (DMG file) to mount it. 
1. Run the `Open Web Start Installer.app`.
1. Choose a language and click **OK** to open the <span class="my-karakun">Open</span>WebStart Setup wizard. 
1. Click **Next** to start the <span class="my-karakun">Open</span>WebStart installation.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click **Next**. 
   <br />Default: `/Applications/Open Web Start`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click **Next**.
1. Please wait for <span class="my-karakun">Open</span>WebStart to be installed on your computer.
1. Click **Finish** on the completion screen to close the wizard.

# How to Use <span class="my-karakun">Open</span>WebStart

<span class="my-karakun">Open</span>WebStart installs an executable called `javaws` that can run Java Web Start apps (.JNLP suffix). 

To run .JNLP applications with <span class="my-karakun">Open</span>WebStart, double-click to open them as usual. 

Alternatively, you can run any webstart app `myApp.jnlp` with <span class="my-karakun">Open</span>WebStart from the command line or terminal:

  * Windows Command Line
  <br />`C:\Program Files\OpenWebStart\javaws -jnlp myApp.jnlp -console`
  * Linux Terminal
  <br /> `/opt/openwebstart/javaws -jnlp myApp.jnlp`

**Note:** If you have an existing Oracle `javaws` executable associated with your .JNLP applications, you need to change the file association for the .jnlp suffix.

## How to change the JNLP file association from Oracle javaws to OpenWebStart javaws

During the development phase, the <span class="my-karakun">Open</span>WebStart installer will not change file associations of any existing Oracle `javaws` executable, so you can use both. 

To associate .JNLP applications with <span class="my-karakun">Open</span>WebStart in Windows Explorer:

1. Right-click the JNLP app and select **Open With -&gt; Choose Another App**.
1. Click **More Apps** and scroll down.
1. Click **Look for Another App on this PC**.
1. Browse to <span class="my-karakun">Open</span>WebStart at `C:\Program Files\OpenWebStart\javaws`.
1. Click **Open** to associate this JNLP file with <span class="my-karakun">Open</span>WebStart.

To associate .JNLP applications with <span class="my-karakun">Open</span>WebStart in the macOS Finder:

1. Right-click the JNLP app and select **Open With -&gt; Other...**.
1. Browse to <span class="my-karakun">Open</span>WebStart at `/Applications/Open Web Start/javaws`.
1. Click **Open** to associate this JNLP file with <span class="my-karakun">Open</span>WebStart.

# How to perform an unattended installation

1. Install <span class="my-karakun">Open</span>WebStart for your operating system as described in this article.
   <br />The installer creates a response file that stores the options that you have chosen in the installer.
1. Locate the response file and copy it next to the <span class="my-karakun">Open</span>WebStart installer:
   * For Windows: `C:\Program Files\OpenWebStart\.install4j\response.varfile`
   * For macOS: `/Applications/Open Web Start/.install4j/response.varfile`
   * For Linux/Unix: `/opt/openwebstart/.install4j/response.varfile`
1. Run the installer again from the command line with the parameter `-q -varfile response.varfile` to execute an unattended installation.
   * For Windows: `OpenWebStart_windows_Setup.exe -q -varfile response.varfile`
   * For macOS: `sudo Open\ Web\ Start\ Installer.app -q -varfile response.varfile`
   * For Debian Linux: `sudo OpenWebStart_linux_0_4_0.deb -q -varfile response.varfile`
   * For Unix: `sudo ./OpenWebStart_unix_0_4_0.sh -q -varfile response.varfile`

# How to Uninstall <span class="my-karakun">Open</span>WebStart

1. Go to your <span class="my-karakun">Open</span>WebStart directory. 
1. Run the Uninstaller.
1. Click **Next** in the <span class="my-karakun">Open</span>WebStart Uninstaller wizard.
1. Wait for the Uninstaller to complete.
1. Click **Finish** on the completion screen to close the wizard.
