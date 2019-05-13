---
layout: article
title: Technical Details
order: '16'
headerText:
permalink: /technical-details/
header:
  text: The functionality of <span class="my-karakun">Open</span>WebStart
nav:
  bottom: false
---

## Technical details
<span class="text-highlight">Open<span>WebStart</span></span> will be based on the JNLP-specification 
defined in [JSR-56](https://www.jcp.org/en/jsr/detail?id=56). It will implement the most commonly used features of Java Web Start and
it will be able to handle any typical JWS-based application. We plan to support all future versions of Java, starting with Java 11. 
In addition to Java 11, the first release of <span class="text-highlight">Open<span>WebStart</span></span> will also support Java 8.

Read on for all the technical details:

### How do I install and manage OpenWebStart?
<span class="text-highlight">Open<span>WebStart</span></span> will come in two different versions:

- An interactive installer with auto-update functionality
- An unattended installer for automated roll-outs

If you use Web Start for several small customers or on your own, we recommend using the __interactive installer__.
Our native installer will set up everything on your Windows, Mac, or Linux system so that <span class="text-highlight">Open<span>WebStart</span></span> is immediately ready to use.
<span class="text-highlight">Open<span>WebStart</span></span> checks for updates automatically, and the Updater component keeps the tool current without the need for any user interaction.

If you or your customers are companies with IT departments of their own, we recommend an __unattended installation__ to roll out <span class="text-highlight">Open<span>WebStart</span></span> on multiple client machines.
In this scenario, the auto-update functionality is inactive; your IT department is free to plan and handle rollouts of new versions based on your internal workflows.

![rollout]({{ "/assets/images/webstart/rollout.png" | relative_url }})


### Which JNLP features will be supported?
Nothing will change from the point of view of your users. <span class="text-highlight">Open<span>WebStart</span></span> will provide exactly the same JNLP-based workflow as Java Web Start:

1. A user either clicks a link on a webpage, or an automated provisioning process downloads a JNLP file to the client. The JNLP file describes the application.
1. <span class="text-highlight">Open<span>WebStart</span></span> registers itself as default for the JNLP file extension and the MIME-type `application/x-java-jnlp-file`. From now on, <span class="text-highlight">Open<span>WebStart</span></span> launches when users double-click any JNLP file.
1. <span class="text-highlight">Open<span>WebStart</span></span> parses the JNLP file, downloads all required resources (JARs, native libraries and images), and stores them in a cache.
1. When all resources are downloaded, the application starts.

![app manager]({{ "/assets/images/webstart/manage-applications.png" | relative_url }})

The included App Manager will manage all JNLP-based application that <span class="text-highlight">Open<span>WebStart</span></span> has downloaded and started. The App Manager checks regularly whether updates are available for its managed applications, and downloads updates automatically.

### Can I manage JDK/JRE versions?
<span class="text-highlight">Open<span>WebStart</span></span> from Karakun will provide an integrated JVM Manager.
The JVM Manager downloads Java versions from a dedicated server, and manages versions internally. With <span class="text-highlight">Open<span>WebStart</span></span>, it will be easy for developers to specify the Java version to run JNLP-based applications.

![JVM management]({{ "/assets/images/webstart/manage-java-version.png" | relative_url }})

By default, <span class="text-highlight">Open<span>WebStart</span></span> will download an OpenJDK-based Java version from a dedicated server. You can also configure servers manually in the <span class="text-highlight">Open<span>WebStart</span></span> Control Panel.

![download JVM]({{ "/assets/images/webstart/download-jvm.png" | relative_url }})

### How do I configure OpenWebStart?
The well-known Java Control Panel that was installed together with Oracle Java was part of Web Start.
When Web Start is removed from Oracle Java, we'll also lose the Control Panel.

This is why <span class="text-highlight">Open<span>WebStart</span></span> comes with its own Control Panel: 
The new Control Panel will, among other things, let you configure workflows to start JNLP-based applications by hand.

### Can I get a customer-specific build?
The free-to-use <span class="text-highlight">Open<span>WebStart</span></span> builds use the default configuration described on this page.

If you want to evaluate <span class="text-highlight">Open<span>WebStart</span></span> without registering the tool for the JNLP MIME-type, 
we can provide you with a build that is configured to use a custom "JNLPX" MIME-type instead.
This allows for an easy migration from Oracle Web Start to <span class="text-highlight">Open<span>WebStart</span></span>.
Additionally, you can customise the server URL for JDK downloads, and provide JDKs for your clients and customers on a custom server.
If you want to use a commercial JDK that is not publically available, you can even configure <span class="text-highlight">Open<span>WebStart</span></span> to use authentication and download JDKs from a secure server.

These are custom configurations that we offer for our customers that have bought commercial support at Karakun. 
Just what you need? Contact us at [OpenWebStart@karakun.com](mailto:openwebstart@karakun.com)!

![rocket]({{ "/assets/images/webstart/rocket.png" | relative_url }})
