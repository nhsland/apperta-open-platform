Apperta Foundation - Defining an Open Platform

6.6 Legacy Connectors
Applications running on an open platform
will need to communicate with existing
systems in health and care that are not
themselves complaint with open platform
principles.
Creating connectors with legacy systems
requires that three distinct aspects are
addressed:

1. Technical and informatics issues;
1. Commercial agreement with system
vendors; and
1. Access agreement with the data
controller and/or data subject and IG.

Where an open platform offers legacy
connectors to its users, it has the potential
to address (at least in some part) all
of these issues. This will present a
significant benefit to the open platform’s
users as it will remove many aspects
that are presently a significant barrier to
application development.

6.6.1 Technical and Informatics issues

1. Technical Issues

Technical issues include technical
mappings and transforms to allow legacy
system connectors to be exposed by way
of a modern API (currently REST with
GraphQL emerging). The mapping may
involve older API technologies on the
legacy system (e.g. SOAP, WSDL, etc.); or
it may involve exposing non-API based
interfaces on legacy systems as a modern API.
Legacy interfaces were often designed for
limited use by a few trusted developers,
and they frequently lack the management,
authentication and cybersecurity
protections required by APIs that may be
exposed to the Internet. An open platform
typically provides an API Management
Gateway that can handle the technical
transformations, provide related open
source adaptors for reuse and provide
the management and protection of the
underlying legacy interface.
2. Informatics Issues
The stages of integration that are possible
on the journey from the current healthcare
IT landscape, with many legacy systems
that struggle to share structured data,
towards a federated set of systems based
on a common architecture, demands
support for a step wise approach. In
exploring a 6 staged maturity model
towards an Integrated Digital Care Record
future, this work may be a useful way to
explore the journey ahead for many of us.
The key informatics challenge towards
a set of consistently modelled record
artefacts is content mapping. This
problem arises because systems represent
similar concepts (e.g. clinical or care data)
in different ways, using different levels
of granularity, and with differing usage of
standard terminologies.
A key feature of an open platform is that
all systems share a common set of open
information models.

24
November 2017

