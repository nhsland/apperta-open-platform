---
title: Open Platform Architecture
permalink: /docs/open-platform-architecture/
comments: true
---
The specific architecture of an implementation of an open platform meeting the
proposed definition will vary from implementation to implementation. However, at a high
conceptual level the architecture will take a form similar to that in the diagram below.

![Open Platform Architecture diagram](/apperta-open-platform/img/doc_images/open-platform-architecture-diagram.png "Open Platform Architecture diagram")

As a minimum the platform provider
will provide a service bus that provides
authentication, routing, and API
management allowing applications to
securely access the APIs provided by
platform service providers.

Optionally, a platform provider may
provide facilities to build or host
applications and platform services; or they
may provide some of the platform services
themselves. The platform provider may
provide federation services to enable
applications to access the data or services
held on other compliant platforms.

A typical platform will have the capability
to support a large number of users running
thousands of applications, and will offer a
number of platform services (typically low
double figures in number).
