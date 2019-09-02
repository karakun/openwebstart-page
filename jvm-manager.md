---
nav:
  bottom: false
  top: false
---  

## JVM Manager

<span class="text-highlight">Open<span>WebStart</span></span> from Karakun will provide an integrated JVM Manager.
The JVM Manager downloads Java versions from a dedicated server, and manages versions internally. 
<span class="text-highlight">Open<span>WebStart</span></span> makes it easy for developers to specify the Java version and vendor to run JNLP-based applications.

You configure the JVM Manager using the  <span class="text-highlight">Open<span>WebStart</span></span> Settings client:

![jvm manager]({{ "/assets/images/webstart/jvm-manager.png" | relative_url }})

Within the JVM Manager Settings panel, a list of all known JVMs is displayed.  
The more options menu (ellipsis) of the list items allows to activate/deactivate and remove a managed JVM instance from the list.

### Local JVMs

To find existing Java installations on your local machine, use the "Find local" option.
All found JVMs are listed and are deactivated by default.
Removing locally installed JVMs from the list does not delete them from the file system.

To manually add local JVM installations to the list, use the "Add local" option. 
This option is very helpful if you have a JVM installed in a non-standard location which is not detected by a "Find local" search.

### Remote JVMs

<span class="text-highlight">Open<span>WebStart</span></span> provides a standard download server with a basic set of popular non-commercial JVMs.
You can set a custom download server in the "Settings" dialog.

By default, <span class="text-highlight">Open<span>WebStart</span></span> will only download JVMs from the configured server.
You can allow the usage of the server specified in the JNLP file by enabling the option "Allow server from JNLP file".

### Additional Settings

The update strategy for remote JVMs can be one of the following:
* Use local if available
* Ask if newer version should be downloaded
* Always download newer version

To narrow down the JVM download and usage of a specific vendor you can select a vendor from the list of provided vendors.
If you don't have any specific vendor preference and want to allow <span class="text-highlight">Open<span>WebStart</span></span> to pick a JVM from any vendor, select the asterisk.
The default vendor is set to "AdoptOpenJDK".

To specify the supported JVM version, provide a valid version string according to [JSR-56, Appendix A](https://www.jcp.org/en/jsr/detail?id=56). 
By default, <span class="text-highlight">Open<span>WebStart</span></span> supports JVMs with version 1.8 and later (1.8+). 

