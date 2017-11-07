Apperta Foundation - Defining an Open Platform - October 2017

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
Apache Thrift would appear to be the API
technologies to watch.
(2) API Actions
There will typically be a small number of
actions (~10) that an application will need
to perform on a given service. What these
actions are will depend on the nature of
the service, but they will typically include
querying, reading and writing data to
and from the service or the control of
transactions managed by the service.

7.2.2 Open APIs that are Currently
Available
The majority of open APIs that have been
developed to-date have been focused on
interactions with electronic health records
(EHRs). Available open APIs of note
include:
•	 openEHR EHRScape API - This
provides comprehensive REST APIs to
any openEHR compliant Clinical Data
Repository (CDR);
•	 HL7 FHIR API - This provides a REST
API to any FHIR compliant EHR;
•	 SMART - This provides a definition of
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
•	 IHE Profiles API Specification This
provides specifications of the APIs for
IHE.

7.2.3 HL7 FHIR
HL7 FHIR is worthy of special reference
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
FHIR profiles developed by INTEROPen

31
November 2017

