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

<span class="my-karakun">Open</span>WebStart alpha comes with a user-friendly installer for Windows. Download the "stable" build to try out the <span class="text-highlight">Open<span>WebStart</span></span> alpha release now!

## How to Install <span class="my-karakun">Open</span>WebStart on Microsoft Windows

1. Go to the [download area](/download) and download `OpenWebStart_windows-x64_0_1_0-alpha.zip`.
1. Run the installer.
1. Choose a language and click **OK** to open the <span class="my-karakun">Open</span>WebStart Setup wizard. 
1. Click **Next** to start the <span class="my-karakun">Open</span>WebStart installation.
1. Browse to the directory where to install <span class="my-karakun">Open</span>WebStart, and click **Next**. 
   <br />Windows default: `C:\Program Files\OpenWebStart`
1. Enable the checkbox to associate the .JNLP suffix with <span class="my-karakun">Open</span>WebStart, and click **Next**.
1. Wait while Setup installs <span class="my-karakun">Open</span>WebStart on your computer.
1. Click **Finish** on the completion screen to close the wizard.

# How to Use <span class="my-karakun">Open</span>WebStart

<span class="my-karakun">Open</span>WebStart installs an executable called `javaws` that can run Java Web Start apps (.JNLP suffix). During the development phase, the <span class="my-karakun">Open</span>WebStart installer will not change file associations of any existing Oracle `javaws` executable, so you can use both.

To run .JNLP applications with <span class="my-karakun">Open</span>WebStart in Windows Explorer:

1. Right-click the JNLP app and select **Open With -&gt; Choose Another App**.
1. Click **More Apps** and scroll down.
1. Click **Look for Another App on this PC**.
1. Browse to <span class="my-karakun">Open</span>WebStart at `C:\Program Files\OpenWebStart\javaws`.
1. Click **Open** to associate this JNLP file with <span class="my-karakun">Open</span>WebStart.

Alternatively, you can run .JNLP applications with `javaws` in the Terminal:
Example: `C:\Program Files\OpenWebStart\javaws -Xnofork -jnlp myApp.jnlp`

# How to Uninstall <span class="my-karakun">Open</span>WebStart

1. Go to your <span class="my-karakun">Open</span>WebStart directory. 
   <br />Windows default: `C:\Program Files\OpenWebStart` by default.
1. Run the Uninstaller.
1. Click **Next** in the <span class="my-karakun">Open</span>WebStart Uninstaller wizard.
1. Wait for the Uninstaller to complete.
1. Click **Finish** on the completion screen to close the wizard.
