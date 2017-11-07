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
