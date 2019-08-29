---
nav:
  bottom: false
  top: false
---  

## JVM Manager

<span class="text-highlight">Open<span>WebStart</span></span> from Karakun will provide an integrated JVM Manager.
The JVM Manager downloads Java versions from a dedicated server, and manages versions internally. 
With <span class="text-highlight">Open<span>WebStart</span></span>, it will be easy for developers to specify the Java version and vendor to run JNLP-based applications.

The JVM Manager is configured using the  <span class="text-highlight">Open<span>WebStart</span></span> Settings client.
Within the JVM Manager Settings panel a list of all known JVMs is displayed.  
The list item menu allows to activate/deactivate and remove a JVM instance from the list.

### Local JVMs

With "Find local" <span class="text-highlight">Open<span>WebStart</span></span> allows to find existing Java installations on your local machine.
All found JVMs are listed and are deactivated by default.
Removing a locally installed JVM from the list does not delete it from the file system.

"Add local" allows to manually add additional local JVM installations to the list. 
For example if the you have JVM installed in a non-standard location which is not detected by a "find local" search.

### Remote JVMs

<span class="text-highlight">Open<span>WebStart</span></span> provides a standard download server with a basic set of non-commercial JVMs.
This can be changed to your preferred custom download server in the "Settings" dialog.
By default, <span class="text-highlight">Open<span>WebStart</span></span> will only download JVMs from the configured server.
You can allow the usage of the server specified in the JNLP file by enabling the option "Allow other servers".

### Additional Settings

The update strategy for remote JVMs can be one of the following:
* Ask for update on local match (default)
* Do nothing on local match
* Automatically download

To narrow down the JVM download and usage of a specific vendor you can select the vendor from the list of provided vendors.
To allow any vendor select the asterisk.
The default vendor is set to "AdoptOpenJDK".

