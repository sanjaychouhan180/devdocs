---
group: config-guide
subgroup: 09_Varnish
title: Install Varnish
menu_title: Install Varnish
menu_order: 5
menu_node:
version: 2.2
github_link: config-guide/varnish/config-varnish-install.md
functional_areas:
  - Configuration
  - System
  - Setup
---

## Install Varnish {#config-varnish-install}
Installing the Varnish software is beyond the scope of this guide. For more information about installing Varnish, see:

*	<a href="http://wiki.mikejung.biz/Varnish" target="_blank">installation wiki</a>
*	<a href="https://www.varnish-cache.org/docs" target="_blank">Varnish installation guides</a>
*	<a href="http://www.tecmint.com/install-varnish-cache-web-accelerator" target="_blank">How to install Varnish (Tecmint)</a>

<div class="bs-callout bs-callout-info" id="info" markdown="1">
This topic is written for Varnish on CentOS and Apache 2.2. If you're setting up Varnish in a different environment, some commands are likely different. Consult the preceding documentation for more information.

If you intend to install Varnish modules (vmods), such as saint mode, you should install Varnish by compiling the code, rather than installing from a package. See [Saint mode]({{ page.baseurl }}/config-guide/varnish/config-varnish-advanced.html#saint) for more details.
</div>

## Confirm your Varnish version {#config-varnish-version}
Enter the following command to display the version of Varnish you're running:

	varnishd -V

A sample follows:

	varnishd (varnish-4.0.3 revision b8c4a34)
	Copyright (c) 2006 Verdens Gang AS
	Copyright (c) 2006-2014 Varnish Software AS

Make sure the version is 4.x or 5.x before continuing. If you are running version 3.x, you must upgrade to a supported version. Consult the Varnish installation documentation for more information.

### Next step
<a href="{{ page.baseurl }}/config-guide/varnish/config-varnish-configure.html">Configure Varnish and your web server</a>
