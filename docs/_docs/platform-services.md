---
title: Platform Services
permalink: /docs/platform-services/
comments: true
---
Apperta Foundation - Defining an Open Platform

6. Platform Services
Platform services provide those facilities
needed to build interoperable health and
social care applications. The platform
services offer those things that app
developers cannot or do not want to do
themselves.
A platform provides access to these
services via secure and robust APIs
(Application Programming Interfaces)
while the services themselves are
designed to provide flexible and scalable
access to the resources required.
The number of platform services that
could be provided is unlimited and will
include services to help developers deal
with both generic technical challenges
and challenges specific to the health
and social care environment. However, a
useful platform can be provided with just
a few services. The concept of a Minimal
Viable open Platform (MVP - the minimum
number of services necessary to provide a
viable open platform) see section 9.
This section lists the classes of service
that might be usefully provided on an

open platform in health and social care.

6.1 Identity Assurance,
Authorisation and
Authentication Services
1. Identity Assurance

Identity Assurance is concerned with
establishing that an individual claiming
a particular identity is that person.
Identity Assurance can be extended to
establishing that the individual has the
status or qualifications they claim (e.g. is
a registered health or care professional
licensed to practice in the UK).
Health and care apps are concerned about
the identity assurance of individuals and
their role(s) in health and care. Identity
can be assured at a number of levels and
is typically achieved by the individual
providing various proofs of identity
and qualifications. This can range from
a simple check that an individual has
control over an email address they use to
identify themselves, through to developed
vetting by the security services. For health

18
November 2017

Apperta Foundation - Defining an Open Platform - October 2017

and care purposes something between
these two extremes is required. An
example candidate is the GOV.UK Verify
service. An open platform may choose to
provide access to this type of service as an
“Assured Identity Service” for its users.
2. Authorisation
Authorisation is concerned with the
authority an individual has. Authorisation
can be described in general terms:

Is individual “I” allowed to perform action
“A” on an object “O”?
This may include i’s authority to access
data or perform an action on a particular
patient or service user. Alternatively,
authorisation might capture a data
subjects consents for particular uses
of data or actions. The rights to grant
authorisations and consents sit with
a multitude of entities including both
individuals and organisations. The open
platform may choose to provide the
assured records of such authorisations as
a “Service” for its users.

### 3. Authentication

Authentication is concerned with
the technical measures that allow
an individual to access and use their
identity credentials, e.g. passwords, keys,
biometrics, etc. Authentication is typically
achieved by proving some combination of
one or more of:

* Something they know - a password or secret;
* Something they have - a key, a smart card, or some other unique device;
and/or
* Something about them - a fingerprint, a voice print or other biometric.

Authentication services are a core part of an open platform implementation.

1919
November
November
2017
2017

Apperta Foundation - Defining an Open Platform

6.2 Data Repositories
An essential component of any open
platform is the provision of data
repositories to store data about patients
and service users who are the subjects of
care, and for these to be held in an open
shareable format. The repositories are
the patient’s own record and have been
variously described as an Electronic
Health Record (EHR), Integrated Digital
Care Record (ICDR), and a Personal Health/
Care Record (PHR/PCR).
Current open platform implementations
typically provide three linked repositories:

* A demographics service, sometimes
described as a registry or master
index containing basic demographic
information about the subject of care.
* A structured data repository A
repository where highly structured
information can be stored in an open
shareable format. By far the most
widely implemented examples of a
structured data repositories are those
based on the openEHR standard.
* A "document" store, sometimes
described as a Vendor Neutral Archive
(VNA). This is a repository to store
documents and other unstructured
or semi-structured data along with
supporting structured metadata.
VNA’s are widely used to store textual
documents or images, but they are
capable of storing anything that
can be represented in any arbitrary
digital format. By far the most widely
implemented examples of a document
store are those based on the IHE-XDS
standard.

A platform providing just the service
bus and a data repository provides the
minimal viable configuration for an open
platform (see section 9).

6.3 Record Locator Services

A record locator service provides an
extension to a demographics service,
enabling records to be located where
there are multiple data repositories on
a single platform implementation or
there is access across multiple federated
platforms implementations.
In the context of the NHS England, a
record locator service is an obvious
extension of the the Spine PDS.

6.4 Resource Discovery and Scheduling

Applications will often need information
about resources available to provide health
and care services and be able to allocate
them or schedule their use for a particular
patient and service user. The scope of
such activities is very wide ranging and
may include:

* Requests for tests and investigations;
* Referrals for advice or treatment;
* GP appointments;
* A nursing home bed; or
* A home care visit.
Apperta Foundation - Defining an Open Platform - October 2017

Health and social care organisations
presently spend significant resources to
both locate and secure suitable resources.
Their methods are commonly manual and
highly inefficient, leading to interruptions
in patient flows, the sub-optimal use
of resources, and avoidable costs and
suffering.
There are potentially a number of platform
services that could be created to assist
with the process of discovering available
resources, allocating them,and scheduling
their use and handling the resultant
financial flows.
There are some existing services that
could be exposed via an open platform of
which the most significant in the NHS for
example is the e-Referral Service.

2121
November
November
2017
2017

Apperta Foundation - Defining an Open Platform

6.5 Knowledge Sources
Applications need to access information
and knowledge in order to function. This
knowledge is highly diverse. At one end of
the spectrum, it includes data that is easily
interpreted and can be easily provided
in the form of simple static lists and
tables. At the other end of the spectrum,
it includes complex representations of
clinical pathways (workflows), decision
support rules and heuristics, and data that
is rapidly changing or difficult to interpret.
Examples include: details or order sets and
test batteries; drug information; resource
availability; clinical terminologies; and
content definitions.
An open platform may provide Knowledge
Sources as “Services” that are accessible
through standard APIs. The Knowledge
Source Services may either simply
return the required data, or in the case
of complex knowledge, the Service may
return a relevant interpretation based
on data provided by the requestor. For
example, a drug knowledge source might
return a specific dosage recommendation
rather than simply the standard dose or
dose range.
There is a vast range of knowledge
sources that could be provided through an
open platform. These include:

6.5.1 Workflow
Services to orchestrate workflow between
applications could bring significant
extra capabilities to an open platform.
Many care pathways cut across multiple
systems and organisations and many
failures of care are the result of poor our

failed handovers between individuals and
organisations on the care pathway.
The effective management of care
pathways that cut across multiple
applications requires open and
computable standards for the
representation and management of
workflows. Currently work in this area is
immature. Generic workflow standards
such as BPMN-2 have the potential to
handle many of the workflows found
in health but can’t handle some of the
many highly complex non-deterministic
workflows found in health and care.
Here specific healthcare standards
such as openEHR’s GDL and PROforma
might provide the required functionality.
openClinical.net provides a working
implementation of PROforma while
openClinical.org provides a good overview
of much of the work in this area

6.5.2 Terminology Services
Terminologies used in health and care
such as SNOMED CT are large and
complex and difficult to implement.
While some developers may require
access to raw terminology data, for many
developers, sophisticated terminology
services are available that have the
potential to handle much of SNOMED CT’s
intrinsic complexity (e.g. equivalence,
subsumption, mapping between
terminologies and the handling of subsets
and resets).

22
November 2017

Apperta Foundation - Defining an Open Platform - October 2017

6.5.3 Clinical Calculators
There are a large number of calculations
made in medicine. Some are simple and
easily handled by developers. Others
are difficult and error-prone, requiring
complex look-ups and adjustments
against multiple factors or normative
datasets (e.g. paediatric weight centiles)
and some are safety critical (e.g. opiates
equivalence calculations).

This data could usefully be made available
via an API. This has been recognised by
the The Organisation Data Service (ODS)
Strategy 2015-2020. However, to-date, there
has been no commitment by the NHS to
implement this strategy recommendation
which will be necessary if these data are
to be made available as an open platform
service.

Quality assured clinical calculators can be
provided as a platform service, removing
both the complexity of the calculation and
management of any associated risks from
the developer.

6.5.6 Drug Information

6.5.4 TRUD Data
The Technology Reference data Update
Distribution site run by NHS Digital
contains a large number of sets of
reference data. These datasets are
available for download and most can
be used free of charge after a simple
registration process.
However many of these could be made
more conveniently available via an API on
the open platform.

Many applications require information
about medicines. The requirement for
drug information includes simple static
data (such as form, strength route and
pack sizes) and more sophisticated active
decision support (relating to such things
as contraindications, interactions, crosssensitivities and dosage). There are freely
available sources for much of the static
data likely to be required (e.g. NHS dm+d).
For comprehensive information, it is
necessary to turn to commercial providers
some of whom have suitable APIs. These
APIs could be made available via an open
platform

6.5.5 Organisation Data Service
The Organisation Data Service run by
NHS Digital contains data about NHS
and partner organisations. This data
is available for download in a machine
readable form (some of the most detailed
information is only available to NHS
users).

23
November 2017

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

Apperta Foundation - Defining an Open Platform - October 2017

Integrated Digital Care Record - Maturity Levels
Shared

View

Published

Modelled

Reconciled

Maturity
Level

Tech Comments

0

Not
Shared

No View

No effective sharing

1

Shared

Diverse
View

HTML view shared

2

Shared

Aligned
View

e.g. XML/JSON shared

3

Shared

Aligned
View

Persisted

4

Shared

Aligned
View

Persisted

Archetyped

5

Shared

Aligned
View

Persisted

Archetyped

e.g. Document Store

25
November 2017

e.g. Medication Records
from GP, Community
Hospital etc
Reconciled

e.g. City Wide Medication
Record

Apperta Foundation - Defining an Open Platform

6.6.2 Commercial Issues
A legacy vendor may not be able to handle
requests from hundreds of app developers
and a small app developer may find it too
difficult to engage with multiple partner
programmes. Some legacy vendors
may also use their position to obstruct
connections that they do not see as in
their commercial interest.

All systems vendors recognise the
importance of interoperability. The
vendor community as a whole knows
that they can grow the total market size
and thus the opportunity for individual
vendors by creating a better Return
on Investment (ROI) for customers
through interoperability. Indeed, it is the
vendor community that has led most
of the successful work in the area of
interoperability (e.g. IHE, HL7 v2, MIG,
INTEROPen) driven by commercial
imperatives to solve interoperability
issues in order to sell systems.
However, it must be recognised that
many established vendors have business
models reliant on customer lock-in and
will resist opening up their systems in a
way that undermines this core business
approach. While they will be supportive
of providing limited APIs such as those
proposed by INTEROPen, they will resist
more fundamental changes to open up all
of the data in their systems, removing the
commercial benefit they currently gain
through data lock-in.
Many vendors have partner programmes
designed to facilitate third parties
wishing to connect to their systems.
As the number of third parties wishing
to connect grows, this “many-to-many
relationship” creates serious problems.
These problems affect both the vendor and
the third party.

An open platform provider can act as
a broker in this relationship, shifting
control over the decision of who connects,
from the legacy vendor and to the data
controller or data subject. We know from
the GPSoC Programme that giving legacy
vendors too much power (for instance
in who connects and how they connect),
severely restricts interoperability.

6.6.3 Access Agreement and
Information Governance
Finally, once technical and commercial
issues are resolved an app developer still
needs permission to connect from the
data controller of the system to which
they wish to connect. The data controller
needs to establish the bonafides of the
user of any connecting application and
where the connection is being approved
on the basis of the data subject's wishes
(as will often be the case for apps used
by patients), that the data subject has
consented.

26
November 2017

Apperta Foundation - Defining an Open Platform

Here too an open platform provider can act
as a broker much simplifying this problem
for the app developer, app user, and data
controller by providing identity assurance
and authentication by either acting as
a trusted third party (itself providing
certifications relating to the app or app
user) or in a trust-agnostic mode (where
it simply provides a gateway to external
source of trust). In addition, by proxying
connections to legacy systems, a platform
can protect underlying systems from
damaging behaviour by an app (either
malicious or unintentional) eliminating
the need for technical accreditation of
apps by end systems vendors

2727
November
November
2017
2017


