### As a GP, should I receive a PEM for every call to NHS 111?

GPs should not be getting a PEM at the end of every call to NHS 111. A message will be received by the GP surgery from NHS 111 if the outcome was ‘For Action’ - this means that the patient has been told to see his or her own GP.

GPs will usually also receive a PEM (notification that a contact has taken place) at the end of every call to NHS 111, except in the following circumstances:

* When a patient is referred to OOH by NHS 111 - the GP , the GP should not receive a PEM as they will eventually receive a ‘PEM’ from the OOH service - this prevents duplication and since implementation has already resulted in a significant reduction in PEMs to GPs.

* When the outcome is on the 'Never Send Disposition' list - NHS 111 systems should suppress all PEMs for the dispositions in this list.

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

Given the nature of these referrals, it is considered that PEMs can be safely suppressed without introducing clinical risk.

In practice the proportion of calls which fall into these disposition categories is small (approx. 1.9%) and so the reduction impact on the overall system is also low.

This list is reviewed as part of each NHS Pathways version release by the Regional Clinical Leads.


### Why doesn't it just use the same system that Out of Hours messaging does?

NHS 111 is a nationally available number and although routing calls is very accurate it cannot be guaranteed that a GP’s patients will be handled by the local 111 service. OOH PEMs do not have a consistent data structure or carrier mechanism, which means the system cannot simply be ‘scaled-up’ to deal with NHS 111 messages. [\*](#footnote1)

### Will I still receive a PEM message if the patient has been directed to me for onward care?

If a patient is told to contact their GP a PEM will be sent that will clearly state this is for action. A second PEM for information should not be received. If either of these are happening then it is a symptom of not using ITK or NHSMail for PEM purposes.

### Why am I receiving Faxes?

A practice may receive a fax if they are not using ITK or NHSMail, this is generally due to one of the practices' patients being handled by an out of area 111 service in another part of the country, perhaps while travelling for work or an occasional misrouting of a call. The service handing the call will always obey the DOS and a lookup will occur, if there is an ITK endpoint or and NHSMail email address it will adhere to it.

However in the event that neither ITK or NHSMail are returned from the DOS the out of area service will not know about any local configuration that the local service may have. This leaves the service little option to meet it's NQR requirements and they will typically fax a version of the PEM to the practice.

Faxes can also occur in the odd event of a technical failure from local 111 services as a contingency mechanism.

### Why am I receiving different versions of PEM?

Firstly if a practice is using ITK then all PEM will be consistent as every 111 service will adhere to it. In the event NHSMail is used then it is up to the sending service to render that message before it is trasmitted. The local version of that renderer may have deviated from the national standard, this is acceptable however services choosing to do this need to factor in they will be causing a variance problem to other practices around the country when dealing with our of area calls.

Faxing is also locally determined and varies greatly across the country as it tends to have a multitude of local variance aligning with out of ours service requirements, systems also give the call handler choice so therefore isn't always system driven and can introduce user error into the equation.

Variance and choice is part of the fundamental standard however it is best implimented after a message has been received via ITK as this will have no impact on any other service and is the recommended approach.

---

<a name="footnote1">* </a> This can be due to border issues, new mobile masts that have not been correctly assigned to the correct area, and other factors which cannot be controlled. Water can also carry mobile phone signals much further distances and make it possible for a mobile mast further away to be connected to a mobile handset.
