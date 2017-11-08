---
title: Standards for an Open Platform
permalink: /docs/standards-for-an-open-platform/
comments: true
---
**Open standards are critical to achieving
the central aim of an open platform** - that
is, portability for data and substitutability
for applications so that neither gets locked
into a particular vendor's platform.

This requires standards in two areas:

* Open Interface standards (APIs); and
* Content standards.

Before turning attention to these
standards, we will consider the difference
between technical and content-based
standards.

### An Understanding of Technical vs Content-based Standards….
Defining suitable open API standards is
primarily a technical problem and is not
a difficult problem to address. **There are
well established standards from the [Open
API Initiative](https://www.openapis.org/). APIs for an open platform
should be defined using these standards.**

#### Content Standards
Content standards define the way in
which the content (often called “clinical
content”) is represented in systems and
interactions between them. Content
standards can be applied to the way
information is stored in an electronic
record or to the payload of a message
or API. Content standards typically
describe how information describing a
particular concept (e.g. A blood pressure
or dementia assessment) should be
formatted, structured and coded to make it
unambiguously computable.

**Defining content is primarily a clinical11
rather than a technical problem.** It is
concerned with getting clinicians to agree
what they mean by a given concept, the
parameters associated with the concept
and how they are represented. This is
work that needs to be led by clinicians
supported by informaticians.

There is much confusion in the area of
interoperability in health and care that
flows from the failure to understand the
difference between technical and content
standards. This confusion is compounded
by the fact that leading standards like HL7
FHIR and openEHR address both technical
and content issues. Nevertheless, the
way they address this is quite different,
with FHIR focusing on a limited range of
content. The consequence is that FHIR
lacks the mature community, governance
and tooling for large scale content
development and maintenance.

Content is ideally defined in a way that
is agnostic to any particular technical
representation. This is particularly
important as content standards tend to
be convergent and stable over the longterm whereas technical standards are
constantly changing.

### Open API Standards
**An open platform appears to applications
as nothing more than a set of open APIs
which enable them to access platform
services.**

The endgame for an open platform
architecture is to have a complete set
of platform microservices for all those
things that can usefully be offloaded to
the platform by the developers’ app. Each
microservice will include a standard
and stable open API expressed using
the standards defined by the [Open API
Initiative](https://www.openapis.org/). The potential number of
platform microservices is potentially
large (maybe some hundreds to a few
thousand). However, the problem is a longtailed one, which means a open platform
with a small number of services (less than
10) can provide high utility to developers.

#### Defining an open API
In defining an open API, an open platform
will require to specify the technical
operation of the API (this is a generic
issue) and the actions that the API
will support (this is a domain specific/
flavoured issue):

##### (1) Technical Operation
API technologies are continually changing
but the current preference amongst
application developers is for REST APIs
carrying a JSON payload. This would be
the current choice of API technology for
an open platform.

However, REST APIs are designed to return
a fixed, predetermined payload. This can
make complex queries (that are common
in the health and care domain) inefficient
and onerous for the developer. The
complex queries will require a subset of
the data from the payloads of many REST
APIs calls. Here new approaches based
on GraphQL12 are gaining currency and
GraphQL and other technologies such as
[Apache Thrift](https://thrift.apache.org/) would appear to be the API
technologies to watch.

##### (2) API Actions
There will typically be a small number of
actions (~10) that an application will need
to perform on a given service. What these
actions are will depend on the nature of
the service, but they will typically include
querying, reading and writing data to
and from the service or the control of
transactions managed by the service.

#### Open APIs that are Currently Available
The majority of open APIs that have been
developed to-date have been focused on
interactions with electronic health records
(EHRs). Available open APIs of note
include:
- [openEHR EHRScape API](https://www.ehrscape.com/api-explorer.html) - This
provides comprehensive REST APIs to
any openEHR compliant Clinical Data
Repository (CDR);
- [HL7 FHIR API](https://www.hl7.org/fhir/http.html) - This provides a REST
API to any FHIR compliant EHR;
- [SMART](https://smarthealthit.org/) - This provides a definition of
a set of openAPIs for EHRs and data
warehouses, to enable app developers
to build apps that will connect to any
SMART enabled system. The current
version of SMART is built on HL7 FHIR.
The use of FHIR simplifies SMART
enablement of systems but limits the
data available to SMART apps to that
available in implemented FHIR profiles
on the underlying system; and
- [IHE Profiles API Specification](http://ihewiki.wustl.edu/wiki/index.php/XDS_Main_Page) - This
provides specifications of the APIs for
IHE.

#### HL7 FHIR
[HL7 FHIR](https://www.hl7.org/fhir/) is worthy of special reference
because of the attractiveness of this
standard to developers and the interest it
has generated in both the global and local
informatics communities.

HL7 FHIR provides a REST API that can be
implemented on any EHR system. FHIR
provides a small number of definitions
for common elements of clinical content
(FHIR Resources) that it carries in a
structured JSON payload. FHIR is well
suited to the provision of a common
open API on EHR systems in a way that
does not require radical changes to the
internal data structures of systems. It was
designed as a messaging standard and
elegantly handles the common messaging
requirements between systems.

HL7 FHIR is an important standard and
any open platform implementation should
support those FHIR profiles that have been
adopted in the care community they cover.
In the UK context this would be those
FHIR profiles developed by [INTEROPen](http://www.interopen.org/)

### Managing Content

#### Defining “Content”
The term “content” (often called “clinical
content) is used to describe the data
elements that make up a health and care
record and the metadata that supports
them (for example, a blood pressure, an
allergy, an assessment, a goal, etc.). These
elements represent the health and care
record in terms of data types, values,
and terminology bindings.The elements
must be computable, open and shareable.
The methodology for defining clinical
content must support the entire lifecycle
of content management, i.e. discovery -->
creation --> peer-review --> publication -->
maintenance.

#### Sharing of Content Facilitating long term Maintenance of Content
Making metadata and content open
and shareable not only facilitates
interoperability but also allows the
increasingly large and burdensome task
of its creation and maintenance to be
shared. Sharing the creation of clinical
content will improve quality and reduce
duplication of effort.

Sharing becomes even more important
with the significant increase in the volume
of content arising from the Internet of
Things, Genomics, personalised medicine,
decision support, data analytics, and
population health. This will result in an
explosive growth in the need for shared
computable definitions of clinical content
from less than 100 that approaches like
FHIR are able to address to nearer 10,000.

**This challenge of both content creation
and ongoing maintenance requires new
approaches and global cooperation.13**
Sharing perhaps represents the only
way that this workload will be able to be
handled.

#### Sharing of Content Stimulating innovation by app developers
Having these elements of content is
also key to enabling new app developers
to innovate without becoming mired
in the complexities of health and care
data. This is a clinical rather than
technical challenge. [This piece by Ewan
Davis](https://www.digitalhealth.net/2016/05/ewan-davis-the-content-challenge/) explains why clinicians rather
than modellers should create clinical
content, drawing on the expertise of
informaticians. The same applies in social
care as it is practitioners not modellers
who need to create and maintain content.

#### Sharing of Content Stimulating interoperability, and supporting scalability
**Current approaches to interoperability
have had limited success, are not scalable
beyond a small set of messages and APIs**,
and do not support the needs of new
entrants to the market, particularly when
these require novel content. The previous
narrow focus on system interoperability
will not support the emerging
requirements which take us from a
“messaging mentality” to what Thomas
Beale describes as “pervasive semantics”
in his blog [here](https://wolandscat.net/2016/04/05/e-health-standards-beyond-messages/).

#### Content Standards
The following standards are potential
candidates for the representation of
clinical content within an open platform:

##### openEHR
[openEHR](http://www.openehr.org/) is the only currently available
open standard14 for the representation of
fine-grained structured clinical content
that is sufficiently mature and proven at
scale and it is thus the only contender
as the standard for the storage of finegrained computable data in an open
platform.

openEHR has a well-established
worldwide community along with a
well-developed set of software tools for
creating and maintaining content. This
puts openEHR in an excellent position
to address the challenge of creating and
curating of fine grained computable
content at scale.

**openEHR has already been adopted as the
national standard for the representation
of clinical content in Norway, India,
Slovenia and Brazil and is used for
standards development in Australia,
Finland, Sweden, Russia, Philippines
and Canada.** openEHR has mature and
open governance arrangements and
an established global community of
clinicians, Informaticians and vendors
coordinated by the not-for-profit openEHR
Foundation based in London. There are a
number of proprietary implementations
of the openEHR standard that have been
deployed at scale15 as well as a number of
promising open source projects. Although
created in London, there has been limited
use of openEHR in the UK with only a
handful of small projects. However, this
is beginning to change with the recent
adoption of openEHR for important
projects including Leeds16, Plymouth17 and
Genomics England18

openEHR also provides the core of the NHS
Digital supported [Code4Health platform](https://platform.code4health.org/#/)
that provides a sandpit environment
where developers and clinicians can
learn about open platform principles and
technologies, enabling them to experiment
to build prototype applications.

##### IHE-XDS
[IHE-XDS](http://wiki.ihe.net/index.php/Cross-Enterprise_Document_Sharing) is an open standard that provides
a mechanism designed for the sharing
of documents and images along with
relevant metadata in a health and care
environment. IHE-XDS provides standards
for vendor neutral archive (VNA) in
which data can be stored in open formats
and a registry which stores metadata
to facilitate data retrieval. Although
primarily used for documents and images,
it can be used for managing any type of
unstructured or semi-structured data.

**IHE-XDS is well supported by the vendor
community and has been used at scale
in many places both standalone and
combination with openEHR.** In the UK,
IHE-XDS has been used to provide the NW
Shared Infrastructure Service LPRES

##### IHE-XDS + openEHR
IHE-XDS and openEHR work well together
and this combination has been used
successfully at scale in both Moscow and
Slovenia. XDS handles unstructured and
semi-structured data while openEHR
handles fine-grained structured data with
links between the openEHR clinical data
repository and the XDS VNA enabling the
creation of a seamless record.

This combination would seem to represent
the most obvious target architecture
where UK local health communities wish
to create an open-platform.

##### Terminologies and SNOMED CT
Terminologies play an important part
in the definition of clinical content and
here the recognised standard is [SNOMED
CT](http://www.snomed.org/snomed-ct) although a platform may need to
support other classification systems both
to support legacy systems’ interfaces
and use cases where SNOMED CT is
not universally used (e.g. [LOINC](https://loinc.org/) which
is used by HL7 FHIR to code laboratory
data). Ideally a platform should provide
terminology services supporting standard
terminologies and locally defined
terminologies along with mechanism to
support mappings between them where
this is relevant. Terminologies and
classification in addition to SNOMED CT
that should be considered include:

- ICD9
- ICD10
- Read 2
- CVT3
- LOINC
- ICPC
- dm+d19

SNOMED CT will be the primary
terminology used in a open platform.
However, there is not a consensus on the
role SNOMED CT should play in particular
the extent to which the use of post
coordinated SNOMED CT expressions is
either practical or desirable. There is a
significant problem: policy makers who
have attempted to mandate the use of
SNOMED CT have little or no idea of its
complexity.
However, the use of SNOMED CT primarily
as a pre-coordinated terminology
is relatively straightforward and
plays an important role in achieving
interoperability.

##### HL7 FHIR
As is stated above (section 7.2.3) HL7
FHIR is an important standard primarily
concerned with the specification of
common open APIs for EHR systems
and it should be supported by any open
platform implementation.

However, while much clinical content
can be satisfactorily represented by FHIR
resources. FHIR is immature (HL7 formally
describe it as a “Standard for Trial Use”)
and it lacks the established methodology,
community, governance and tooling to
enable its use creating and curating of
fine grained computable content at scale
and is not suitable as the prime means of
representing clinical content in an open
platform ecosystem.

FHIR was designed to support
interoperability between systems and
focuses on a small number of profiles
to support common interoperability
requirements. It was not intended as
a format for the storage of data within
systems or as a mechanism for large scale
clinical content creation and curation.

It is proposed that clinical content
development should focus on openEHR
where the established methodology,
community, governance and tooling exist
and that the output of this work is used
in the creation of FHIR resources and
profiles where these are required.This blog
by Thomas Beale [explains](https://wolandscat.net/2016/04/10/openehr-technical-basics-for-hl7-and-fhir-users/) how FHIR and
openEHR can work together.

#### User Interface (UI) and User Experience (UX) standards and frameworks

##### Vision
The vision of an open digital ecosystem
is that any end user will be able to select
a unique set of applications drawn from
multiple vendors, where each applications
will meet the end user’s unique needs,
and where each application will work
seamlessly together. The application
should be:

- Interoperable - Able to share relevant
data between themselves;
- Orchestrated - Work together;
- Form-factor agile - Adapt their UI to the
form-factor of the device they are used
on; and
- UI/UX consistent - Operating with a
common look and feel.

We make the case for open standards,
components and frameworks at the UX/UI
level of an open platform, very well aware
of the generally poor level of usability in
healthcare IT, mindful of the unnecessary
cognitive load this puts on already busy
clinicians at the frontline.

In the same way that stepping into a rental
car generally results in the driver easily
finding the common components required
to steer, accelerate, brake, indicate, etc
as they are placed in a highly consistent
manner across the automotive industry,
we believe there now is a compelling case
for a common usability framework in
healthcare.

Attention to clinical safety is one of the
bywords for good practice in modern
healthcare and any inspection of the
people/process/technology challenge
when seeing the varied UX landscape
across a typical healthcare environment
quickly explains why we have [the rate
of medical errors that are so problematic
today](https://www.theguardian.com/society/2016/dec/31/serious-mistakes-nhs-patient-care-rising-figures-reveal-hospitals).

##### Achieving the Vision
Achieving this vision of an open digital
ecosystem that has a consistent UX/UI is
non-trivial. It requires the development
of standards and frameworks that will
support developers to build applications
that achieve these objectives.

It is possible to draw analogies here from
other sectors. For example the open
source Wordpress content management
system (CMS) provides a core “platform”
which can be augmented with plug-ins
from multiple vendors (as of May 2017,
there are over 50,000 Wordpress plugins)
to create a unique website. By separating
the UI components into “themes”, a site
built with plugins from multiple vendors
can be given a consistent UI/UX by
applying an appropriate theme of which
there are many thousands to choose from.

The ultimate aim is to see a number of
such frameworks developed that provide
similar capabilities for application
developers in health and care. In the world
of CMSs there are of course frameworks
other than Wordpress, and the same can
be expected in health and care.

#### A starting point for a health and care frameworks…..
There are a number of generic frameworks
that can be used to create a consistent
UI/UX. While these would require work to
satisfy the full needs of health and care,
they offer significant flexibility and could
be augmented with specific health and
care specific UI components. Frameworks
of note include:

* [Bootstrap](http://getbootstrap.com/);
* [Angular JS](https://angularjs.org/);
* [React](https://reactjs.org/);
* [Semantic UI](https://semantic-ui.com/)

What all of these frameworks have in
common is that they are open source
projects created by leading Internet
companies (Twitter, Facebook, Google
and Pivotal) all of whom recognise that
by open sourcing their tools they gain
much more than they give away. These
companies also recognise the need to
do so in a way that allows commercial
exploitation of the frameworks by others
(each framework is released using a
commercial friendly licence).

Some years ago there was some beautiful
UX work done in the US as part a [Health
Design Challenge](http://healthdesignchallenge.com/), which yielded a range
of new UX ideas for healthcare.
Some other related and relevant work
within the NHS in England. This included
the [NHS Common User Interface (CUI)
Project](https://digital.nhs.uk/common-user-interface) - This is work from the NPfIT.
Whilst it is no longer maintained, it
provides a starting point of good practice
and principles.

While these efforts have explored new
UX possibilities in healthcare, there
is a paucity of open source UX/UI
frameworks that have been implemented
for healthcare.To address this, the [Ripple
Foundation](http://ripple.foundation/) - (non profit organisation who
are promoting an open integrated health
and care platform compatible with the
definition proposed in this document)
have built and supported several related
components including an open source
patterns & component based UX/
UI framework called [PulseTile](http://ripple.foundation/pulsetile/) which
appears to be a leading example of the
way ahead.
