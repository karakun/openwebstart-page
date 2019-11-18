---
layout: article
title: Predefined configuration
order: '16'
headerText:
permalink: /configuration/
header:
  image: webstart-2
  text: Predefined configuration for <span class="my-karakun">Open</span>WebStart
hidden: true
nav:
  bottom: false
---
When installing <span class="my-karakun">Open</span>WebStart, several properties can be predefined in a so-called `response.varfile` file.

Some of the supported properties are lockable. If a property is lockable, you can define an additional property of type `PROPERTY_NAME.locked=true` to prevent users from editing the property in the user interface. For example, to define a value for the `ows.jvm.manager.server.default` property that cannot be changed in the user interface, specify the following two properties:

{% highlight plaintext %}
ows.jvm.manager.server.default=https://my.custom.server
ows.jvm.manager.server.default.locked=true
{% endhighlight %}

The following table provides an overview of all properties that can be specified in the `response.varfile`:

{% assign lockableIcon = '<span class="icon has-text-success"><i class="fas fa-lg fa-check-square"></i></span>' %}

{:.table}
| property            | lockable                                                   | description                |
| ------------------- | ---------------------------------------------------------- | -------------------------- |
{% for property in site.data.config-properties -%}
| {{property.name}} |  {%- if property.lockable -%} {{lockableIcon}} {%- endif -%} | {{ property.description }} |
{% endfor -%}
| | | |

To create a `response.varfile` file, run the installation of <span class="my-karakun">Open</span>WebStart at least once manually. By doing so a `response.varfile` file is created in <span class="my-karakun">Open</span>WebStart installation folder in your system. In the installation folder, you find a `.install4j` folder that contains the basic `response.varfile` file. The content of such a file looks like this:

{% highlight plaintext %}
# install4j response file for OpenWebStart 1.0.0-SNAPSHOT
sys.adminRights$Boolean=false
sys.fileAssociation.extensions$StringArray="jnlp","jnlpx"
sys.fileAssociation.launchers$StringArray="313","313"
sys.installationDir=/Applications/OpenWebStart
sys.languageId=de
{% endhighlight %}

You can easily edit this file and add additional properties based on the table in this article. Do not change the initial content of the file, and add new properties always to the end of the file. After editing, a `response.varfile` file might look like this:

{% highlight plaintext %}
# install4j response file for OpenWebStart 1.0.0-SNAPSHOT
sys.adminRights$Boolean=false
sys.fileAssociation.extensions$StringArray="jnlp","jnlpx"
sys.fileAssociation.launchers$StringArray="313","313"
sys.installationDir=/Applications/OpenWebStart
sys.languageId=de
ows.jvm.manager.server.default=https://my.custom.server
ows.jvm.manager.server.default.locked=true
{% endhighlight %}

If you now use such a file to install <span class="my-karakun">Open</span>WebStart, all the properties will be automatically imported and used at the first start of <span class="my-karakun">Open</span>WebStart.
