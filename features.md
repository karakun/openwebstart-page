---
layout: article
title: Features
order: '12'
permalink: /feature-table/
header:
  text: <span class="my-karakun">Open</span>WebStart Features
nav:
  bottom: true
---

## Features
This is the list of features of <span class="text-highlight">Open<span>WebStart</span></span> that we are going to implement, with their priority and their current state.
You can download the current version in the [download area](/download).

<table class="feature-table">
<tr>
    <th>Identifier</th>
    <th>Feature</th>
    <th>Priority</th>
    <th>Description</th>
</tr>

<tr>
    <th colspan="4">Installation & Administration</th>
</tr>

<tr class="feature-done">
    <td>INST-1</td>
    <td>Windows installer</td>
    <td>1</td>
    <td>Native installer for Windows</td>
</tr>
<tr class="feature-done">
    <td>INST-2</td>
    <td>Mac installer</td>
    <td>1</td>
    <td>Native installer for Mac</td>
</tr>
<tr class="feature-done">
    <td>INST-3</td>
    <td>Linux installer</td>
    <td>1</td>
    <td>DEB-package</td>
</tr>
<tr class="feature-done">
    <td>INST-4</td>
    <td>Unattended installer for Windows</td>
    <td>1</td>
    <td>One needs to be able to run the installer in unattended mode</td>
</tr>
<tr class="feature-done">
    <td>INST-5</td>
    <td>Unattended installer for Linux</td>
    <td>1</td>
    <td>One needs to be able to run the installer in unattended mode</td>
</tr>
<tr class="feature-done">
    <td>INST-6</td>
    <td>Unattended installer for Mac</td>
    <td>1</td>
    <td>One needs to be able to run the installer in unattended mode</td>
</tr>
<tr class="feature-done">
    <td>INST-7</td>
    <td>File extension and MIME type registration</td>
    <td>1</td>
    <td>
        The default MIME type and file extension that should be associated with a JNLP file:<br/>
        Default MIME Type: application/x-java-jnlp-file<br/>
        Default Extension: .jnlp<br/>
        JSR-56, Ch. 3.2
    </td>
</tr>
<tr class="feature-missing">
    <td>INST-8</td>
    <td>OpenWebStart Updater</td>
    <td>1</td>
    <td>
        Checks for updates, downloads and installs new versions automatically or on demand. It must be possible to deactivate the update-mechanism since it should not be used by companies that do the rollout themselves.
    </td>
</tr>
<tr class="feature-done">
    <td>INST-9</td>
    <td>Control Panel</td>
    <td>1</td>
    <td>GUI to configure the different modules of OpenWebStart</td>
</tr>
<tr class="feature-removed">
    <td>INST-10</td>
    <td>Removed</td>
    <td>1</td>
    <td>This requirement has been removed.</td>
</tr>
<tr class="feature-partially">
    <td>INST-11</td>
    <td>Configuration by property file</td>
    <td>1</td>
    <td>
        All configuration properties can be defined in an external file to define unmodifiable values. By defining properties in such a file the user can not modify the properties in the configuration UI of OpenWebStart.
    </td>
</tr>
<tr class="feature-done">
    <td>INST-12</td>
    <td>Custom Mime-Type</td>
    <td>1</td>
    <td>
        When installing OpenWebStart the user can define if he wants the tool to be registered for the .jnlp / application/x-java-jnlp-file mime type or if he wants to use a different mimetype (jnlpx). This allows to run OpenWebStart in parallel to JavaWebStart. This can only be defined when installing OpenWebStart. To change this definition the tool needs to be reinstalled.<br/>
        JSR-56, Ch. 3.2
    </td>
</tr>
<tr class="feature-done">
    <td>INST-13</td>
    <td>Shell support</td>
    <td>1</td>
    <td>
        The tool can be started (at least with a -v and -help parameter) from the shell.<br/>
        The -version parameter will print the current version of the tool<br/>
        The -help parameter will print an install help text
    </td>
</tr>

<tr>
    <th colspan="4">Application Manager</th>
</tr>

<tr class="feature-done">
    <td>AM-1</td>
    <td>Cache Management</td>
    <td>1</td>
    <td>
        Provide a cache for all applications downloaded by the user. The cache can be managed by the user.<br/>
        JSR-56, Ch. 6.5<br/>
        JSR-56, Ch. 6.6
    </td>
</tr>
<tr class="feature-partially">
    <td>AM-2</td>
    <td>Application Updates</td>
    <td>1</td>
    <td>
        Check for cached applications if there is a newer version, if so, the new version is updated either incrementally or completely. We will support HTTP and HTTPS as protocol.<br/>
        JSR-56, Ch. 6<br/>
        JSR-56, Ch. 3.4<br/>
        JSR-56, Ch. 3.6:<br/>
        Initially we will only support the parameter types:<br/>
        check-attribute=always<br/>
        policy-attribute=always
    </td>
</tr>
<tr class="feature-missing">
    <td>AM-3</td>
    <td>Background Updates</td>
    <td>1</td>
    <td>
        OpenWebStart allows to update applications in the background while the current version of the application is running. After the download is finished the new version becomes available with the next restart of the application.<br/>
        JSR-56, Ch. 3.6<br/>
        check-attribute=background
    </td>
</tr>
<tr class="feature-missing">
    <td>AM-4</td>
    <td>Incremental Updates</td>
    <td>1</td>
    <td>
        OpenWebStart supports the download of JARDiff files (JARDiff = tool to visualise API differences between two different versions of a project, takes two jar files and outputs all the public API changes as xml, html or plain text)<br/>
        JSR-56, Ch. 6.3.1<br/>
        JSR-56, Appendix B
    </td>
</tr>
<tr class="feature-done">
    <td>AM-5</td>
    <td>Native Lib Support</td>
    <td>1</td>
    <td>
        OpenWebStart supports the usage of native libraries in the application<br/>
        JSR-56, Ch. 4.3
    </td>
</tr>
<tr class="feature-done">
    <td>AM-6</td>
    <td>Offline Support</td>
    <td>1</td>
    <td>
        Applications can be started offline. There is a check whether all resources (with its correct versions) are available in the application cache.<br/>
        JSR-56, Ch. 5.1.1
    </td>
</tr>
<tr class="feature-done">
    <td>AM-7</td>
    <td>Application Resources Download</td>
    <td>1</td>
    <td>
        OpenWebStart can download application resources  (JARs, images, ...) as specified in the JNLP file.<br/> 
        Such resources will be part of the application and automatically downloaded.<br/>
        Such resources can be restricted to a specific operating system, architecture, or locale using the os, arch, and locale attributes<br/>
        JSR-56, Ch. 4.1<br/>
        JSR-56, Ch. 4.3
    </td>
</tr>
<tr class="feature-low-priority">
    <td>AM-8</td>
    <td>Lazy Download of Resources</td>
    <td>2</td>
    <td>
        The JNLP file download attribute is used to control whether a resource is downloaded eagerly or lazily.<br/>
        JSR-56, Ch. 4.4
    </td>
</tr>
<tr class="feature-partially">
    <td>AM-9</td>
    <td>Versioning of Resources</td>
    <td>1</td>
    <td>
        Resources can be versioned.<br/>
        JSR-56, Ch. 6<br/>
        JSR-56, Ch. 6.5.2
    </td>
</tr>
<tr class="feature-done">
    <td>AM-10</td>
    <td>System Properties</td>
    <td>1</td>
    <td>
        System properties (OS dependend) can be set and processed in JNLP.<br/>
        JSR-56, Ch. 4.2
    </td>
</tr>
<tr class="feature-done">
    <td>AM-11</td>
    <td>Clear Cache</td>
    <td>1</td>
    <td>The application cache can be cleared by the user.</td>
</tr>
<tr class="feature-done">
    <td>AM-12</td>
    <td>Versioning of JNLP files</td>
    <td>1</td>
    <td>
        JNLP files can be defined with a version attribute. This helps to check if an JNLP based application is updated.
    </td>
</tr>
<tr class="feature-partially">
    <td>AM-13</td>
    <td>Installation on Windows</td>
    <td>1</td>
    <td>
        OpenWebStart can install an application according to the preferences specified in the descriptor information.<br/>
        JSR-56, Ch. 3.5<br/>
        We will support:
        <ul>
            <li>Desktop Shortcut</li>
            <li>Start Menu Entry</li>
            <li>Default MIME type and file extension association</li>
        </ul>
        The details on how the integration can be established depend on the OS.
    </td>
</tr>
<tr class="feature-low-priority">
    <td>AM-14</td>
    <td>Installation on Linux</td>
    <td>2</td>
    <td>
        OpenWebStart can install an application according to the preferences specified in the descriptor information.<br/>
        JSR-56, Ch. 3.5<br/>
        We will support:
        <ul>
            <li>Default MIME type and file extension association</li>
        </ul>
        The details on how the integration can be established depend on the OS.
    </td>
</tr>
<tr class="feature-missing">
    <td>AM-15</td>
    <td>Installation on Mac</td>
    <td>1</td>
    <td>
        OpenWebStart can install an application according to the preferences specified in the descriptor information.<br/>
        JSR-56, Ch. 3.5<br/>
        We will support:
        <ul>
            <li>Start Menu Entry</li>
            <li>Default MIME type and file extension association</li>
        </ul>
        The details on how the integration can be established depend on the OS.
    </td>
</tr>
<tr class="feature-done">
    <td>AM-16</td>
    <td>Application Start</td>
    <td>1</td>
    <td>
        Read .JNLP files of type &quot;application descriptor&quot; and start them according to these description.<br/>
        The general workflow of an application start launch sequence is defined by:<br/>
        JSR-56, Ch. 5.1
    </td>
</tr>
<tr class="feature-done">
    <td>AM-17</td>
    <td>Extension Support</td>
    <td>1</td>
    <td>
        Extension support as defined in the JNLP specification<br/>
        JSR-56, Ch. 3.8<br/>
        JSR-56, Ch. 4.7<br/>
        JSR-56, Ch. 5.7
    </td>
</tr>
<tr class="feature-done">
    <td>AM-18</td>
    <td>Application Descriptors</td>
    <td>1</td>
    <td>
        OpenWebStart supports Application Descriptors in the JNLP file. Only the &quot;application-desc&quot; will be supported as we do not want to support Applets<br/>
        JSR-56, Ch. 3.7
    </td>
</tr>
<tr class="feature-low-priority">
    <td>AM-19</td>
    <td>Auto-cleanup</td>
    <td>2</td>
    <td>OpenWebStart will automatically delete cached applications that are not used for a long time (maybe 6 month?)</td>
</tr>
<tr class="feature-done">
    <td>AM-20</td>
    <td>Java Console</td>
    <td>1</td>
    <td>Show the Java Console for applications</td>
</tr>
<tr class="feature-low-priority">
    <td>AM-21</td>
    <td>Package definition</td>
    <td>2</td>
    <td>
        Specific used packages for Jars can be defined by the JSR definition. We do not think that OpenWebStart should support that.<br/>
        JSR-56, Ch. 4.5
    </td>
</tr>
<tr class="feature-low-priority">
    <td>AM-22</td>
    <td>Pack200</td>
    <td>2</td>
    <td>
        OpenWebStart supports pack200 jar artefact compression. The appropiate accept-encoding header value is &quot;pack200-gzip&quot;<br/>
        This feature will be marked as deprecated and removed in a future version.
    </td>
</tr>

<tr>
    <th colspan="4">JVM Manager</th>
</tr>

<tr class="feature-partially">
    <td>JM-1</td>
    <td>Version Management</td>
    <td>1</td>
    <td>
        OpenWebStart can manage several JVM instances internally. Here the tool has its internal directory in that JVM instances are managed. Such instances are not really installed on the local system (like adding it to the PATH environment variable). The JVM instances are only used and managed by OpenWebStart internally to start JNLP based applications.<br/>
        We do not think that the initial version definition of the JSR is sufficient enough. We plan to provide additional attributes for the JNLP XML syntax to specify supported Java version (version, vendor...)<br/>
        JSR-56, Ch. 4.6
    </td>
</tr>
<tr class="feature-done">
    <td>JM-2</td>
    <td>Update Management</td>
    <td>1</td>
    <td>
        OpenWebStart can check if it has a JVM instances that matches to the needs of a JLNP application. If not OpenWebStart will automatically download a new JVM version that can be used to start the JNLP application.
    </td>
</tr>
<tr class="feature-done">
    <td>JM-3</td>
    <td>Download-Server Management</td>
    <td>1</td>
    <td>
        Since OpenWebStart can download new JVM instances the list of endpoints that can be used to get new JVMs must be specified. Here we need to define a REST API that can be used to ask endpoints for JVMs and than download them. We will support HTTP and HTTPS as protocol.
    </td>
</tr>
<tr class="feature-done">
    <td>JM-4</td>
    <td>Support of vendor-specific JVMs</td>
    <td>1</td>
    <td>
        As some users will have commercial support of a specific JDK vendor it must be possible to define the vendor for a managed JVM.
    </td>
</tr>
<tr class="feature-missing">
    <td>JM-5</td>
    <td>Auto clean</td>
    <td>1</td>
    <td>
        As OpenWebStart will automatically download JDKs we need a mechanism to remove old JDKs once they are not needed anymore (maybe after they are not used for a year).
    </td>
</tr>
<tr class="feature-partially">
    <td>JM-6</td>
    <td>JVM parameters for application start</td>
    <td>1</td>
    <td>
        Several JVM parameters can be specified for an application.<br/>
        JSR-56, Ch. 4.6
    </td>
</tr>

<tr>
    <th colspan="4">JNLP</th>
</tr>

<tr class="feature-done">
    <td>JNLP-1</td>
    <td>JNLP Parser & Verifier</td>
    <td>1</td>
    <td>
        OpenWebStart must parse and verify JNLP files and check its syntax against the JNLP File Document Type Definition<br/>
        JSR-56, Appendix C<br/>
        The parser will know all defined XML attributes of the JNLP standard. If and where such attributes are used by OpenWebStart is defined in other topics of this document.<br/>
        JSR-56, Ch. 3.3
    </td>
</tr>
<tr class="feature-done">
    <td>JNLP-2</td>
    <td>Version IDs and Version Strings</td>
    <td>1</td>
    <td>
        Implementation of the formal syntax of the version-ids and version strings according to JSR-56, Appendix A
    </td>
</tr>
<tr class="feature-done">
    <td>JNLP-3</td>
    <td>Component Extension Support</td>
    <td>1</td>
    <td>OpenWebStart supports to include JNLP files in other JNLP files.</td>
</tr>
<tr class="feature-low-priority">
    <td>JNLP-4</td>
    <td>Deployment Rule Set (Servers)</td>
    <td>2</td>
    <td>Provide depolyment rule set as white list for OpenWebStart resources (URIs).</td>
</tr>

<tr>
    <th colspan="4">Security</th>
</tr>

<tr class="feature-done">
    <td>SEC-1</td>
    <td>Signature Check</td>
    <td>1</td>
    <td>
        OpenWebStart validates the signing of the downloaded JARs.<br/>
        JSR-56, Ch. 5.4<br/>
        JSR-56, Ch. 5.3
    </td>
</tr>
<tr class="feature-low-priority">
    <td>SEC-2</td>
    <td>Untrusted Environment</td>
    <td>2</td>
    <td>
        OpenWebStart allows to start an application in an untrusted environment.<br/>
        JSR-56, Ch. 5.5<br/>
        JSR-56, Ch. 5.3
    </td>
</tr>
<tr class="feature-done">
    <td>SEC-3</td>
    <td>
        Trusted Environment<br/>
        (all-permissions)
    </td>
    <td>1</td>
    <td>
        OpenWebStart allows to start an application in an all-permissions environment.<br/>
        JSR-56, Ch. 5.6<br/>
        JSR-56, Ch. 5.3
    </td>
</tr>
<tr class="feature-low-priority">
    <td>SEC-4</td>
    <td>
        Trusted Environment<br/> 
        (j2ee-application-client)
    </td>
    <td>2</td>
    <td>
        OpenWebStart allows to start an application in an j2ee-application-client environment.<br/>
        JSR-56, Ch. 5.6<br/>
        JSR-56, Ch. 5.3
    </td>
</tr>
<tr class="feature-low-priority">
    <td>SEC-5</td>
    <td>Deployment Rule Set (Certificates)</td>
    <td>2</td>
    <td>Provide deployment rule set as white list for SHA256 hashes/certificates.</td>
</tr>
<tr class="feature-done">
    <td>SEC-6</td>
    <td>Signature Check Deactivation</td>
    <td>1</td>
    <td>OpenWebStart allows to deactivate the signature check, e.g. for in-house applications.</td>
</tr>
<tr class="feature-missing">
    <td>SEC-7</td>
    <td>Server White List</td>
    <td>1</td>
    <td>The list of hosts from where to load code can be restricted.</td>
</tr>
<tr class="feature-done">
    <td>SEC-8</td>
    <td>Proxy Settings</td>
    <td>1</td>
    <td>
        Specify and manage proxy settings.<br/>
        JSR-56, Ch. 5.3"
    </td>
</tr>

<tr>
    <th colspan="4">JNLP Java API</th>
</tr>

<tr class="feature-done">
    <td>JNLP-API-1</td>
    <td>BasicService</td>
    <td>1</td>
    <td>Provide service implementation for querying and interacting with the environment.</td>
</tr>
<tr class="feature-done">
    <td>JNLP-API-2</td>
    <td>DownloadService</td>
    <td>1</td>
    <td>Provide service implementation that allows an application to control how its own resources are cached.</td>
</tr>
<tr class="feature-done">
    <td>JNLP-API-3</td>
    <td>FileOpenService</td>
    <td>1</td>
    <td>Provide service implementation for importing files from the local disk.</td>
</tr>
<tr class="feature-done">
    <td>JNLP-API-4</td>
    <td>FileSaveService]</td>
    <td>1</td>
    <td>Provide service implementation for exporting files to the local disk.</td>
</tr>
<tr class="feature-done">
    <td>JNLP-API-5</td>
    <td>ClipboardService</td>
    <td>1</td>
    <td>Provide service implementation for accessing the shared system-wide clipboard.</td>
</tr>
<tr class="feature-done">
    <td>JNLP-API-6</td>
    <td>PrintService</td>
    <td>1</td>
    <td>Provide service implementation to access printing and submit a print job.</td>
</tr>
<tr class="feature-low-priority">
    <td>JNLP-API-7</td>
    <td>PersistenceService</td>
    <td>2</td>
    <td>Provide service implementation for storing data locally on the client system.</td>
</tr>
<tr class="feature-low-priority">
    <td>JNLP-API-8</td>
    <td>ExtensionInstallerService</td>
    <td>2</td>
    <td>Provide service implementation to communicate with the JNLP Client used by an extension installer.</td>
</tr>
<tr class="feature-done">
    <td>JNLP-API-9</td>
    <td>SingleInstanceService</td>
    <td>2</td>
    <td>
        Provide service implementation for applications to register themselves as singletons, and to register listener(s) for handling arguments passed in from different instances of applications.
    </td>
</tr>
<tr class="feature-partially">
    <td>JNLP-API-10</td>
    <td>ExtendedService</td>
    <td>1</td>
    <td>Provides additional support to the current JNLP API. It allows applications to open specific file(s) in the client's file system.</td>
</tr>
<tr class="feature-low-priority">
    <td>JNLP-API-11</td>
    <td>IntegrationService</td>
    <td>2</td>
    <td>Provide service implementation for programmatic management (create, delete) of desktop and menu shortcuts.</td>
</tr>
<tr class="feature-missing">
    <td>JNLP-API-12</td>
    <td>DownloadService2</td>
    <td>1</td>
    <td>Provide service implementation that allows an application to control how its own resources are cached.</td>
</tr>

</table>

<p/>

Legend: 
<table class="legend-table">
<tr>
    <td class="feature-done">Feature done</td>
    <td class="feature-partially">Feature partially done</td>
    <td class="feature-missing">Feature missing</td>
    <td class="feature-low-priority">Low priority feature</td>
</tr>
</table>

