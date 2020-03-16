---
layout: article
header:
  text: Run <span class="my-karakun">Web Start</span> based application after the release of <span class="my-karakun">Java 11</span>
---

<div class="latest-news">
<h4>Latest news</h4>
<em>16. March 2020:</em><br/>
We just released OpenWebStart 1.1.6.
This release provides improvements when using OpenWebStart in centralized environments and doing unattended installations. It also fixes a bug appeared in v1.1.5 that prevents properly reading the server white list. See also the release notes on <a href="https://github.com/karakun/OpenWebStart/releases" target="_blank">github</a> for further details.
</div>

## Java Web Start is dead. Long live Java Web Start!
Java Web Start (JWS) was deprecated in Java 9, and starting with Java 11, Oracle removed JWS from their JDK distributions.
This means that clients that have the latest version of Java installed can no longer use JWS-based applications.
And since public support of Java 8 has ended in Q2/2019, companies no longer get any updates and security fixes for Java Web Start.

This is why we decided to create <span class="text-highlight">Open<span>WebStart</span></span>, an open source reimplementation of the Java Web Start technology.
Our replacement will provide the most commonly used features of Java Web Start and the JNLP standard, 
so that your customers can continue using applications based on Java Web Start and JNLP without any change.

For more information about the removal of Java Web Start, have a look at these documents:

* [Official Java desktop roadmap from Oracle](https://www.oracle.com/technetwork/java/javase/javaclientroadmapupdate2018mar-4414431.pdf)
* [DZone article about the consequences for Java desktop applications](https://dzone.com/articles/what-the-future-java-releases-will-mean-for-legacy)
* [Do I need to pay for Java now?](https://dev.karakun.com/java/2018/06/25/java-releases.html)

![divider]({{ "/assets/images/webstart/divider-2.png" | relative_url }})

### Enjoy premium support!
Java and your operating system get updates, and so does <span class="text-highlight">Open<span>WebStart</span></span>.
We always have your back with current developments: talk to us about a support subscription at [OpenWebStart@karakun.com](mailto:openwebstart@karakun.com).

### We keep you in the loop!
Want to learn more and stay up-to-date with the project?

<a class="button is-medium full-width-button is-primary" href="/subscribe/">Subscribe to our newsletter</a>

### What does OpenWebStart include?
The main focus of <span class="text-highlight">Open<span>WebStart</span></span> is the execution of JNLP-based applications.
Additionally, the tool contains four modules that simplify your Web Start workflows
and let you configure <span class="text-highlight">Open<span>WebStart</span></span> to suit your needs:

- The **App Manager** manages the versions of any JNLP-based application that is executed by <span class="text-highlight">Open<span>WebStart</span></span>.
- The [**JVM Manager**](/jvm-manager) manages Java versions and Java updates on the client.
- The **Control Panel** provides a graphical user interface to configure <span class="text-highlight">Open<span>WebStart</span></span>.
- The **Updater** downloads and installs new versions of <span class="text-highlight">Open<span>WebStart</span></span>.

You’re a developer and want to take a closer look at our source repo? [Visit our GitHub](https://github.com/karakun/openwebstart) and let us know what you think.
 
### OpenWebStart Roadmap
We have been able to secure a good part of the required funding, and 
we and our sponsors are currently discussing the list of features that we are going to implement.
Our goal is to have the final release 1.0 ready in November.

The following diagram shows the roadmap:

![roadmap]({{ "/assets/images/webstart/roadmap-karakun.png" | relative_url }})

![rocket]({{ "/assets/images/webstart/rocket.png" | relative_url }})
