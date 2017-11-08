---
title: Proposed Definition of an Open Platform
permalink: /docs/proposed-definition-of-an-open-platform/
comments: true
---
### Introduction
When trying to define an open platform it
is necessary to understand the needs of
the different stakeholder groups, as well as
the generic and underlying functionalities
of health and care software applications.

### What do Health and Care Applications do?
At an abstract level all health and care
applications do either or both of the
following:
1. Support the processes that deliver care;
and/or
1. Collect and/or analyse data to support
the delivery of care.

At a functional level, all health and care
applications:
1. Create, consume and update
information about the subjects of care i.e. the health and care record;
1. Consume and process knowledge i.e. data, metadata, care pathways,
decision support rules and heuristics,
etc.; and
1. Manage the consumption of care
resources - (this includes creating,
consuming, processing and updating
information about them - i.e. referrals,
orders, treatments, and services).

Most applications don’t directly create
knowledge, but by collecting data through
the care process they can support
activities that refine current knowledge
and create new knowledge.

### How do Users want to use Applications?
An individual user who is involved in
the health and care system (patient or
service user, family or informal carer or
health and care worker or professional)
would like to be able to choose a set of
applications from multiple vendors that
best support their needs.

An open platform enables applications
from multiple vendors to be orchestrated
to work together to meet an individual
user’s needs.

### What do Developers want from a Platform?
Developers want to focus on writing the
front end applications. They would like to
be able to call upon ready made resources
and services (via API calls) that are
supplied by the platform. These resources
are provided by an open platform as
described above.

### Healthcare Payers and Providers?
Healthcare payers seek lower costs, better
value and a more agile response from
solution providers to their changing needs.

They wish to be able to choose the best
options from multiple vendors and to be
able to move easily when the best option
changes.

They wish to ensure that they can use
their data as they wish and are not be
constrained by it being locked-in to
proprietary formats or systems.

An open platform facilitates agile
development of healthcare apps and
solutions, takes advantage of the lower
cost of cloud infrastructure, eliminates
vendor lock-in and encourages
competition.

### Proposed Definition
The following definition is based on a one
previously proposed6 with amendments
based on feedback from a number of
interested parties.

> In health and care, an open digital
ecosystem can make it easier to
build applications that support
safe, high quality compassionate
care. It allows applications and
services from multiple vendors
to work together for an individual
user whatever their role (e.g.
clinician, patient, carer, social
worker, commissioner, manager,
care worker, etc.) such that there is
a many-to-many substitutability
between applications and services.
In other words, an application
requiring a service can use any
available service provider via
common APIs.
An open ecosystem is vendor and
technology neutral and eliminates
lock-in, facilitates innovation
and forces vendors to compete on
quality, value, and service.

An open platform adheres to the following
principles in order to meet the need of all
stakeholders:
1. **Open Standards Based** -
The implementation should be based on
agile open standards7. Any willing
party should be able to use these
standards without charge to build an
independent, compliant instance of the
complete platform;
1. **Shared Common Information Models** -
There should be a set of common
information models8 in use by all
instances of the open platform,
independent of any given technical
implementation;
1. **Supporting Application Portability** -
Applications written to run on one
platform implementation should be
able to run with either trivial or no
change on another platform that has
been independently developed;
1. **Federatable** -
It should be possible
to connect any implementation of
the open platform to all others that
were independently developed, in
a federated structure, to allow the
sharing of appropriate information and
workflows between them;
1. **Vendor and Technology Neutral** -
The standards should not depend
on particular technologies or require
components from particular vendors.
Anyone building an implementation of
the open platform may elect to use any
available technology and may choose
to include or exclude proprietary
components;
1. **Supporting Open Data** - Data should
be exposed as needed (subject to good
information governance practice) in
an open, shareable, computable format
in near to real-time. Implementors
may choose to use this format natively
in their persistence (storage) layer of
the open platform itself or meet this
requirement by using mappings and
transformations from some other open
or proprietary format;
1. **Providing Open APIs** - The full
specification of the APIs (the means by
which applications are connected to
the platform) should be freely available.
1. **Operability (as in DevOps9)** - The
platform should support the principles
of operability10 (this is all about the
qualities of a systems that enables
applications to operate well throughout
their full life cycle). Software systems
which follow software operability
good practice will tend to be simpler to
operate and maintain, with a reduced
cost of ownership, and almost certainly
fewer operational problems.
