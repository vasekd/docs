---
layout: default
---
Foxx reference
==============

Each Foxx service is defined by a [JSON manifest](foxx-reference-manifest.html)
specifying the entry point, any scripts defined by the service,
possible [configuration](foxx-reference-configuration.html) options and Foxx dependencies,
as well as other metadata. Within a service, these options are exposed as the
[service context](foxx-reference-context.html), which is also used to mount
[routers](foxx-reference-routers-readme.html) defining the service's API endpoints.

Foxx also provides a number of [utility modules](foxx-reference-modules-readme.html)
as well as a flexible [sessions middleware](foxx-reference-sessions-readme.html)
with different transport and storage mechanisms.

Foxx services can be installed and managed over the Web-UI or through
ArangoDB's [HTTP API](../../../HTTP/Foxx/Management.html).