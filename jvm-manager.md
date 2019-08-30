---
nav:
  bottom: false
  top: false
---  

## JVM Manager

<span class="text-highlight">Open<span>WebStart</span></span> from Karakun will provide an integrated JVM Manager.
The JVM Manager downloads Java versions from a dedicated server, and manages versions internally. 
With <span class="text-highlight">Open<span>WebStart</span></span>, it will be easy for developers to specify the Java version and vendor to run JNLP-based applications.

The JVM Manager is configured using the  <span class="text-highlight">Open<span>WebStart</span></span> Settings client:

![jvm manager]({{ "/assets/images/webstart/jvm-manager.png" | relative_url }})

Within the JVM Manager Settings panel a list of all known JVMs is displayed.  
The list item (sandwich) menu allows to activate/deactivate and remove a managed JVM instance from the list.

### Local JVMs

With the "Find local" option <span class="text-highlight">Open<span>WebStart</span></span> allows to find existing Java installations on your local machine.
All found JVMs are listed and are deactivated by default.
Removing locally installed JVMs from the list does not delete it from the file system.

The "Add local" option allows to manually add additional local JVM installations to the list. 
This is very helpful if you have a JVM installed in a non-standard location which is not detected by a "Find local" search.

### Remote JVMs

<span class="text-highlight">Open<span>WebStart</span></span> provides a standard download server with a basic set of popular non-commercial JVMs.
This can be changed to your preferred custom download server in the "Settings" dialog.

By default, <span class="text-highlight">Open<span>WebStart</span></span> will only download JVMs from the configured server.
You can allow the usage of the server specified in the JNLP file by enabling the option "Allow server from JNLP file".

### Additional Settings

The update strategy for remote JVMs can be one of the following:
* Use local if available
* Ask if newer version should be downloaded
* Always download newer version

To narrow down the JVM download and usage of a specific vendor you can select a vendor from the list of provided vendors.
If you don't have any specific vendor preference and want to allow <span class="text-highlight">Open<span>WebStart</span></span> to pick a JVM from any vendor select the asterisk.
The default vendor is set to "AdoptOpenJDK".

The supported JVM version can be specified by providing a valid version string according to [JSR-56, Appendix A](https://www.jcp.org/en/jsr/detail?id=56). 
By default, <span class="text-highlight">Open<span>WebStart</span></span> supports JVMs with version 1.8 and later (1.8+). 

