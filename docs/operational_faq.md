### As a GP, should I receive a PEM for every call to NHS 111?

A [PEM](./glossary.md#pem) will be received by the GP surgery from NHS 111 if the outcome was ‘For Action’ - this means that the patient has been told to see his or her own GP.

GPs will usually also receive a [PEM](./glossary.md#pem) at the end of every call to NHS 111, except in the following circumstances:

* When a patient is referred to OOH by NHS 111 - the GP will receive a [PEM](./glossary.md#pem) as they will eventually receive a [PEM](./glossary.md#pem) from the OOH service - this prevents duplication and since implementation has already resulted in a significant reduction in PEMs to GPs.

* When the outcome is on the 'Never Send Disposition' list - NHS 111 systems should suppress all [PEM](./glossary.md#pem)s for the [dispositions](./glossary.md#disposition) in this list.

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

Given the nature of these referrals, it is considered that [PEM](./glossary.md#pem)s can be safely suppressed without introducing clinical risk.

In practice the proportion of calls which fall into these disposition categories is small (approx. 1.9%) and so the reduction impact on the overall system is also low.

This list is reviewed as part of each NHS Pathways version release by the Regional Clinical Leads.


### Why doesn't it just use the same system that Out of Hours messaging does?

NHS 111 is a nationally available number and although routing calls is very accurate it cannot be guaranteed that a GP’s patients will be handled by the local 111 service. OOH [PEM](./glossary.md#pem)s do not have a consistent data structure or carrier mechanism, which means the system cannot simply be ‘scaled-up’ to deal with NHS 111 messages. [\*](#footnote1)

### Will I still receive a PEM message if the patient has been directed to me for onward care?

If a patient is told to contact their GP a [PEM](./glossary.md#pem) will be sent that will clearly state this is for action. A second [PEM](./glossary.md#pem) for information should not be received. If either of these are happening then it is a symptom of not using [ITK](./glossary.md#itk) or NHSMail for PEM purposes.

### Why am I receiving Faxes?

A practice may receive a fax if they are not using [ITK](./glossary.md#itk) or NHSMail, this is generally due to one of the practices' patients being handled by an out of area 111 service in another part of the country, perhaps while travelling for work or an occasional misrouting of a call. The service handing the call will always obey the [DOS](./glossary.md#dos) and a lookup will occur, if there is an ITK endpoint or and NHSMail email address it will adhere to it.

However in the event that neither [ITK](./glossary.md#itk) or NHSMail are returned from the [DOS](./glossary.md#dos) the out of area service will not know about any local configuration that the local service may have. This leaves the service little option to meet it's [NQR](./glossary.md#nqr) requirements and they will typically fax a version of the [PEM](./glossary.md#pem) to the practice.

Faxes can also occur in the odd event of a technical failure from local 111 services as a contingency mechanism.

### Why am I receiving different versions of PEM?

Firstly if a practice is using [ITK](./glossary.md#itk) then all [PEM](./glossary.md#pem) will be consistent as every 111 service will adhere to it. In the event NHSMail is used then it is up to the sending service to render that message before it is trasmitted. The local version of that renderer may have deviated from the national standard, this is acceptable however services choosing to do this need to factor in they will be causing a variance problem to other practices around the country when dealing with our of area calls.

Faxing is also locally determined and varies greatly across the country as it tends to have a multitude of local variance aligning with out of ours service requirements, systems also give the call handler choice so therefore isn't always system driven and can introduce user error into the equation.

Variance and choice is part of the fundamental standard however it is best implimented after a message has been received via [ITK](./glossary.md#itk) as this will have no impact on any other service and is the recommended approach.

---

<a name="footnote1">* </a> This can be due to border confusion / overlap, newly installed mobile masts that have not yet been assigned to the correct geographical area, and other environmental factors which cannot be controlled.
