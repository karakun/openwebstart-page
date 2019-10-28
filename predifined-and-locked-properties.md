---
layout: article
title: Predefinied configuration
order: '16'
headerText:
permalink: /configuration/
header:
  image: webstart-2
  text: Predefinied configuration for <span class="my-karakun">Open</span>WebStart
hidden: true
nav:
  bottom: false
---
When installing OpenWebStart several properties can be prededined in a so called `response.varfile` file. The File must be passed to the installer by the following command:

{% highlight properties %}
TODO COMMAND
{% endhighlight %}

Some of the supported properties are lockable. If a property is lockable you can define an additional property of type `PROPERTY_NAME.locked=true` to lock the editing of the property in the ui. For the `ows.jvm.manager.server.default` property you can for example specifiy the following 2 properties to define a value that can not changed in the ui:

{% highlight properties %}
ows.jvm.manager.server.default=https://my.custom.server
ows.jvm.manager.server.default.locked=true
{% endhighlight %}

The following table gives an overview of all properties that can be specified in the `response.varfile`:

{% assign lockableIcon = '<span class="icon has-text-success"><i class="fas fa-lg fa-check-square"></i></span>' %}

{:.table}
| property            | lockable                                                   | description                |
| ------------------- | ---------------------------------------------------------- | -------------------------- |
{% for property in site.data.config-properties -%}
| {{property.name}} |  {%- if property.lockable -%} {{lockableIcon}} {%- endif -%} | {{ property.description }} |
{% endfor -%}
| | | |

To create a `response.varfile` file you need to run the installation of OpenWebStart at least once by hand. By doing so a `response.varfile` file will be created in the folder of the installed OpenWebStart on you system. In the installation folder you can find a `.install4j` folder that contains the basic `response.varfile` file. The content of such file looks like this:

{% highlight properties %}
# install4j response file for OpenWebStart 0.5.0-SNAPSHOT
sys.adminRights$Boolean=false
sys.fileAssociation.extensions$StringArray="jnlp","jnlpx"
sys.fileAssociation.launchers$StringArray="313","313"
sys.installationDir=/Applications/OpenWebStart
sys.languageId=de
{% endhighlight %}

You can easily edit this file and add additional properties based on the table below. The initial content of the file should not be changed and new properties should always be added to the end of the file. After mutation a `response.varfile` file might look like this:

{% highlight properties %}
# install4j response file for OpenWebStart 0.5.0-SNAPSHOT
sys.adminRights$Boolean=false
sys.fileAssociation.extensions$StringArray="jnlp","jnlpx"
sys.fileAssociation.launchers$StringArray="313","313"
sys.installationDir=/Applications/OpenWebStart
sys.languageId=de
ows.jvm.manager.server.default=https://my.custom.server
ows.jvm.manager.server.default.locked=true
{% endhighlight %}

If you now use such file to install OpenWebStart all the properties will be automatically imported and used at the first start of OpenWebStart.