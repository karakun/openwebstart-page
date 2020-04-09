---
layout: article
header:
  text: Run <span class="my-karakun">Web Start</span> based application after the release of <span class="my-karakun">Java 11</span>
nav:
  bottom: false
  
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

This is why we decided to create <span class="text-highlight">Open<span>WebStart</span></span>, an open source reimplementation of the Java Web Start technology. Our replacement provides the most commonly used features of Java Web Start and the JNLP standard, 
so that your customers can continue using applications based on Java Web Start and JNLP without any change.

The main focus of <span class="text-highlight">Open<span>WebStart</span></span> is the execution of JNLP-based applications.
Additionally, the tool contains four modules that simplify your Web Start workflows
and let you configure <span class="text-highlight">Open<span>WebStart</span></span> to suit your needs:

- The **App Manager** manages the versions of any JNLP-based application that is executed by <span class="text-highlight">Open<span>WebStart</span></span>.
- The [**JVM Manager**](/jvm-manager) manages Java versions and Java updates on the client.
- The **Control Panel** provides a graphical user interface to configure <span class="text-highlight">Open<span>WebStart</span></span>.
- The **Updater** downloads and installs new versions of <span class="text-highlight">Open<span>WebStart</span></span>.

You’re a developer and want to take a closer look at our source repo? [Visit our GitHub](https://github.com/karakun/openwebstart) and let us know what you think.

![divider]({{ "/assets/images/webstart/divider-2.png" | relative_url }})

### Support the OpenWebStart project
Java and your operating system get updates, and so does OpenWebStart. Thanks to the support of our [awesome
sponsors](/sponsors), OpenWebStart will be updated and further developed as long as needed.

You can of course use <span class="text-highlight">Open<span>WebStart</span></span> as an open source solution free of charge but we‘d also like to talk to you about support options to guarantee the lasting development.

<div class="boxes teaser highlight">
  <div>
  	<span class="boxes-heading">Community Support</span>
	<ul>
		<li>Report bugs using the GitHub Issue Tracker</li>
		<li>Bugs are fixed as soon as possible</li>
	</ul>
	</div>
  <div>
  	<span class="boxes-heading">Basic Support & Sponsoring</span>
	<ul>
		<li>Special communication channel to report bugs</li>
		<li>Bugs have a higher priority but no guaranteed service levels</li>
		<li>10% discount for development of individual features</li>
		<li>Company logo can be published on OpenWebStart sponsor page (basic sponsor)</li>
	</ul>
		</div>
  <div>
  	<span class="boxes-heading">Premium Support & Sponsoring</span>
	<ul>
		<li>Premium communication channel for bug reports</li>
		<li>Bugs have highest priority</li>
		<li>Guaranteed service levels depending on severity of bug (during business hours)</li>
		<li>After bug fix, we provide a corresponding release</li>
		<li>25% discount for development of individual features</li>
		<li>Company logo can be published on OpenWebStart sponsor page (premium sponsor)</li>
	</ul>
		</div>
</div>

Talk to us about your individual support package at [OpenWebStart@karakun.com](mailto:openwebstart@karakun.com).

![divider]({{ "/assets/images/webstart/divider-2.png" | relative_url }})

### We keep you in the loop!
Want to learn more and stay up-to-date with the project?

<a class="button is-medium full-width-button is-primary" href="/subscribe/">Subscribe to our newsletter</a>