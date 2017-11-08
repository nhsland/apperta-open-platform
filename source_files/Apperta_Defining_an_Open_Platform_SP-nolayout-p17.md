Apperta Foundation - Defining an Open Platform - October 2017

5. Open Platform Architecture
The specific architecture of an implementation of an open platform meeting the
proposed definition will vary from implementation to implementation. However, at a high
conceptual level the architecture will take a form similar to that in the diagram below.
Applications ‘000s

API(s)
Federation

Service Bus - Authentication - Routing - API Management

Federation

API(s)

Platform Services ‘0s

As a minimum the platform provider
will provide a service bus that provides
authentication, routing, and API
management allowing applications to
securely access the APIs provided by
platform service providers.

themselves. The platform provider may
provide federation services to enable
applications to access the data or services
held on other compliant platforms.

Optionally, a platform provider may
provide facilities to build or host
applications and platform services; or they
may provide some of the platform services

A typical platform will have the capability
to support a large number of users running
thousands of applications, and will offer a
number of platform services (typically low
double figures in number).

17
November 2017

