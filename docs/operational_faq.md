<a name="q1"></a>
### As a GP, should I receive a PEM for every call to NHS 111?

A [PEM](./glossary.md#pem) will be received by the GP surgery from NHS 111 if the outcome was ‘For Action’ - this means that the patient has been told to see their own GP.

GPs will receive a [PEM](./glossary.md#pem) at the end of every call to NHS 111, except in the following circumstances:

* a patient is referred to OOH by NHS 111, the GP will recieve a [PEM](./glossary.md#pem) from the OOH service - this prevents duplication and since implementation has already resulted in a significant reduction in PEMs to GPs
* the outcome is on the 'Never Send Disposition' list - NHS 111 systems should suppress all [PEM](./glossary.md#pem)s for the [dispositions](./glossary.md#disposition) in this list

The current 'Never Send Disposition' list is:

|||
|-|-|
|DX 28|Contact Pharmacist|
|DX 52|Refer to Police|
|DX 60|Contact Optician next routine appointment within 72 hours|
|DX 22|To be seen by Dental Practice within 3 working days|
|DX 23|Contact Orthodontist next working day|
|DX 45|Provide Service Location Information|
|DX 46|Refer to Health Information|
|DX 63|Refer to Fluline|

Given the nature of these referrals, [PEM](./glossary.md#pem)s can be safely suppressed without introducing clinical risk.

In practice, the proportion of calls which fall into these disposition categories is small (approx. 1.9%) and so the reduction of the number of [PEM](./glossary.md#pem)s sent to GPs also low.

This list is reviewed as part of each NHS Pathways version release by the Regional Clinical Leads.

### Why doesn't 111 just use the same system that Out of Hours messaging does?

NHS 111 is a nationally available number and while routing calls is very accurate, it is not always the case that a GP’s patients will be handled by the local 111 service. OOH [PEM](./glossary.md#pem)s do not have a consistent data structure or carrier mechanism, which means the system cannot simply be ‘scaled-up’ to deal with NHS 111 messages. 

### Will I still receive a PEM message if the patient has been directed to me for onward care?

See [*As a GP, should I receive a PEM for every call to NHS 111?*](#q1)

### Why am I receiving Faxes?

A practice may receive a fax if they are not using [ITK](./glossary.md#itk) or NHSMail, or if a practice's patient is handled by a 111 service in another part of the country. The service handing the call will always obey the [DOS](./glossary.md#dos) and a lookup will occur, and if there is an ITK endpoint or and NHSMail email address it will adhere to it.

In the event that neither [ITK](./glossary.md#itk) or NHSMail are returned from the [DOS](./glossary.md#dos), the out of area service will not know about any local configurations that might exist. This leaves the out of area service little option to meet its [NQR](./glossary.md#nqr) requirements and they will typically fax a version of the [PEM](./glossary.md#pem) to the practice.

Faxes can also occur in the event of a technical failure from local 111 services as a contingency mechanism.

### Why am I receiving different versions of PEM?

If a practice is using [ITK](./glossary.md#itk) then all [PEM](./glossary.md#pem) will be consistent as every 111 service will adhere to it. 

If a practice is using NHSMail, then it is up to the sending service to render that message before it is trasmitted. The local version of that renderer may have deviated from the national standard. It is possible for practices to choose to deviate from the national standard. However, they should understand that doing this will mean that dealing with out of area calls from other practices is harder.  

The choice of whether faxing is used is made by local services and varies across the country. 111 systems also give the call handler choice of whether to use it, and this can introduce error. 

Variance and choice is part of the fundamental standard. The recommended approach is that messages should first be received via [ITK](./glossary.md#itk), as this will have no impact on any other service. At that point practices can vary their approach to handling PEMs. 

---
