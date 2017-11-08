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

