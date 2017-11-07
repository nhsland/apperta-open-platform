Apperta Foundation - Defining an Open Platform

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

IHE-XDS has been used to provide the NW
Shared Infrastructure Service LPRES

openEHR also provides the core of the NHS
Digital supported Code4Health platform
that provides a sandpit environment
where developers and clinicians can
learn about open platform principles and
technologies, enabling them to experiment
to build prototype applications.

This combination would seem to represent
the most obvious target architecture
where UK local health communities wish
to create an open-platform.

7.3.5.2 IHE-XDS
IHE-XDS is an open standard that provides
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
IHE-XDS is well supported by the vendor
community and has been used at scale
in many places both standalone and
combination with openEHR. In the UK,

7.3.5.3 IHE-XDS + openEHR
IHE-XDS and openEHR work well together
and this combination has been used
successfully at scale in both Moscow and
Slovenia. XDS handles unstructured and
semi-structured data while openEHR
handles fine-grained structured data with
links between the openEHR clinical data
repository and the XDS VNA enabling the
creation of a seamless record.

7.3.5.4 Terminologies and SNOMED CT
Terminologies play an important part
in the definition of clinical content and
here the recognised standard is SNOMED
CT although a platform may need to
support other classification systems both
to support legacy systems’ interfaces
and use cases where SNOMED CT is
not universally used (e.g. LOINC which
is used by HL7 FHIR to code laboratory
data). Ideally a platform should provide
terminology services supporting standard
terminologies and locally defined
terminologies along with mechanism to
support mappings between them where
this is relevant. Terminologies and
classification in addition to SNOMED CT
that should be considered include:

* ICD9
* ICD10

34
October 2017

