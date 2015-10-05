### As a GP, should I receive a PEM for every call to NHS 111?

GPs should not be getting a PEM at the end of every call to NHS 111. A message should be received from NHS 111 if the outcome was ‘For Action’ - this means that the patient has been told to see their own GP.

When a patient is referred to OOH by NHS 111, the GP should not receive a PEM as they will eventually receive one from the OOH service - this prevents duplication and since implementation has already resulted in a significant reduction in PEMs to GPs.

There is also a 'Never Send Disposition' list - NHS 111 systems should suppress all PEMs for the dispositions in this list.

The current list is:

* DX 28 – Contact Pharmacist
* DX 52 – Refer to Police
* DX 60 – Contact Optician next routine appointment within 72 hours
* DX 22 – To be seen by Dental Practice within 3 working days
* DX 23 – Contact Orthodontist next working day
* DX 45 – Provide Service Location Information
* DX 46 – Refer to Health Information
* DX 63 – Refer to Fluline

Given the nature of these referrals, it is considered that PEMs can be safely suppressed without introducing clinical risk.

In practice the proportion of calls which fall into these disposition categories is small (approx. 1.9%) and so the reduction impact on the overall system is also low.

This list is reviewed as part of each NHS Pathways version release by the Regional Clinical Leads.


### Why doesn't it just use the same system that Out of Hours messaging does?

This relates to the fact that NHS 111 is a nationally available number, although routing calls is very accurate it cannot be guaranteed that a GP’s patients will be handled by the local 111 service. This can be due to border issues, new mobile masts that haven't been assigned to the area they are in and other factors that cannot be controlled. Water can also carry mobile phone signals much further distances and make it possible for a mobile mast further away to be connected to a mobile handset.


### Will I still receive a PEM message if the patient has been referred to me for onward care?
TBC

### Why am I receiving Faxes?

A practice may receive a fax if they are not using ITK or NHSMail, this is generally due to one of the practices' patients being handled by an out of area 111 service in another part of the country, perhaps while travelling for work or an occasional misrouting of a call. The service handing the call will always obey the DOS and a lookup will occur, if there is an ITK endpoint or and NHSMail email address it will adhere to it.

However in the event that neither ITK or NHSMail are returned from the DOS the out of area service will not know about any local configuration that the local service may have. This leaves the service little option to meet it's NQR requirements and they will typically fax a version of the PEM to the practice.

Faxes can also occur in the odd event of a technical failure from local 111 services as a contingency mechanism.

### Why am I receiving different versions of PEM?
TBC
