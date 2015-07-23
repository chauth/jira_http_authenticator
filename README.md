JIRA HTTP Authenticator
=====

### Overview

This is a port of the [Confluence HTTP Authenticator](https://github.com/chauth/confluence_http_authenticator ) that has hooks to work with the JIRA auth system. The package works much like its Confluence counterpart using Seraph entry points.  

### Build / Install

For now, refer to the various [Confluence](https://github.com/chauth/confluence_http_authenticator) install docs when you get stuck. This will at a minimum give you something to get started with.

Currently use of this authenticator plugin requires knowledge of setting up and using a [maven](http://maven.apache.org) build environment. Please familiarize yourself with [maven](http://maven.apache.org) before moving forward with your use of this plugin. 

#### Build

```
mvn clean

mvn install

```

### Instal

* This plugin does not support installation via Plugin Repository/Plugins in Confluence. You will simply get an error and the plugin will not work.
* Copy the jar file above into JIRA's WEB-INF/lib directory (and if it exists backup existing file). Be sure to note the version of your JIRA install and use the appropriate jar. 
* Copy the sample [properties][config] file into JIRA's WEB-INF/classes directory (and if it exists backup existing file).
* This plugin requires that the Shibboleth SP, Apache, Tomcat, and plugin are setup and configured correctly. 

### Release Notes

See the git log [CHANGELOG][changelog].

### Disclaimer

Docs are limited at the moment. 
This software is available as is. 

### Licence

Copyright (c) 2008-2014, Confluence HTTP Authenticator Team, released under a [BSD-style License][lic].

[changelog]: http://github.com/chauth/jira_http_authenticator/blob/master/CHANGELOG.md
[confluence]: http://github.com/chauth/confluence_http_authenticator/
[lic]: http://github.com/chuath/jira_http_authenticator/blob/master/LICENSE
[config]: http://github.com/chauth/jira_http_authenticator/master/conf/

