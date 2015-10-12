<dl>

<dt><a name="cda">CDA</a></dt>
Clinical Document Architecture
This is a set of standards for HL7 messages. It provides structure and integrity to messages transmitted from one computer system to another. The system recieving the messages uses the standard to inspect the message and understand how it's structured. 

<dt><a name="dos">DOS</a></dt>
Directory Of Services

<dt><a name="disposition">Disposition</a></dt>
A disposition is a ...

<dt><a name="dts">DTS</a></dt>
Data Transfer Service.
This is a mechanism for moving data, typically Kettering messages, from one computer system to another. It works much the same way as email, where a sending system sends the message to a central server which stores it until it is retrieved by the receiving system. The recieving systems usually retrieve messages by 8.00am. 

<dt><a name="hscic">HSCIC</a></dt>
Health and Social Care Information Centre

<dt>ITK</dt>
Interoperability Tool Kit.
This is a standard for moving messages from one computer system to another and is an alternative to DTS. 111 uses a subset of the ITK standards for sending information. 

It is synchronus, which means that it is able to notify the sending system when a message has been successfully delivered, after the recieving system has acknowledged that is has the data. DTS is unable to do this as it uses an intermediary server.

<dt><a name="kettering">Kettering</a></dt>
Kettering is a standard message format that Out of Hours services use to report back to GPs. 

The standard has not been maintained and there are now many variants of it in use. 111 providers don't know which version is being used where, and therefore can't send electronic PEMs to practices that are out of area. In these circumstances, they fall back to fax. 

<dt><a name="nqr">NQR</a></dt>
National Quality Requirement

<dt><a name="pem">PEM</a></dt>
Post Event Messaging
In the context of NHS 111 is an electronic document that is transmitted to GP practices at the end of an NHS 111 contact to notifiy that a contact has taken place. 

There are essentially two types of PEM a GP can receive: 
* ‘For Action’ meaning a GP has been referred back to their own GP with a timeframe associated with it
* ‘For Your Information’ message which is for the GP to inspect and file against the patients record.

<dt><a name="renderedpem">Rendered PEM</a></dt>
Rendered PEM means 'Rendered Post Event Message'
This refers to a CDA document which has been converted from XML format (designed for processing by software) to a human-readable format such as PDF or HTML.
<a href="../technical_faq#renderedpem">Full Explanation of Rendered PEM</a>

<dt><a name="trud">TRUD</a></dt>
Terminology Reference data Update Distribution site 
This is a website that the Health and Social Care Information Centre uses to distribute specifications and resources to be used for NHS Information Technology e.g.
  <ul>
  <li>Messaging Specifications</li>
  <li>Clinical Code Lists</li>
  <li>Accreditation Guidance....</li>
  </ul>
You can access the TRUD Website here: <a href="https://isd.hscic.gov.uk/">https://isd.hscic.gov.uk</a>
