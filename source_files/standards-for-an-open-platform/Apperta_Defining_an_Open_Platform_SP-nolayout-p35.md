Apperta Foundation - Defining an Open Platform - October 2017

* Read 2
* CVT3
* LOINC
* ICPC
* dm+d19

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

It is proposed that clinical content
development should focus on openEHR
where the established methodology,
community, governance and tooling exist
and that the output of this work is used
in the creation of FHIR resources and
profiles where these are required.This blog
by Thomas Beale explains how FHIR and
openEHR can work together.

7.3.5.5 HL7 FHIR
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
35
November 2017

