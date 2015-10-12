<dl>

  <dt><a name="cda">CDA</a></dt>
  <dd>CDA is short for Clinical Document Architecture. It is a set of standards applied to HL7 messages to provide structure and integrity to the messages that are transmitted from one computer system to another. The receiving system is able to inspect these and know exactly what information is contained where. They do need to be populated with quality content.</dd>

  <dt><a name="dos">DOS</a></dt>
  <dd>Directory Of Services</dd>

  <dt>DTS</dt>
  <dd>DTS stands for **Data Transport Service**. It is a mechanism for moving data, typically kettering from one computer system to another. It works much the same way as email, where a sending system sends the message to a central server which stores it until it is retrieved by the receiving system, typically by 08:00 each day.</dd>

  <dt><a name="hscic">HSCIC</a></dt>
  <dd>HSCIC stands for the <b>H</b>ealth and <b>S</b>ocial <b>C</b>are <b>I</b>nformation <b>C</b>entre.<dd>

  <dt>ITK</dt>
  <dd>ITK is the acronym for HSCIC’s Interoperability Toolkit. It’s a standard for how systems talk to each other and is an alternate transport mechanism to DTS. 111 uses a subset of the ITK standards for sending information. The benefit is that it is synchronous, meaning that the sender is notified that the delivery was successful and the recipient has acknowledged they have the data. DTS is not able to do this as their is an intermediary server involved.</dd>

  <dt><a name="kettering">Kettering</a></dt>
  <dd>Kettering is a standard message format that Out of Hours services use to report back to GP’s. The issue with the standard is that it wasn’t maintained and now there are many variants of that standard. This has developed by evolution over a long time and has become fragmented. This is a problem for NHS 111 providers as they are unable to determine what versions are being sent to where making it difficult to send an electronic PEM for patients that are out of area. This would force the 111 provider into faxing the report which has a wide range of quality, is difficult to manage and is more expensive on both parties.</dd>

  <dt><a name="pem">PEM</a></dt>
  <dd>Post Event Messaging (PEM) in the context of NHS 111 is an electronic document, that is transmitted to GP practices at the end of an NHS 111 Call. There are essentially two types of PEM a GP can receive, one that is ‘for action’ meaning a GP has been referred back to their own GP with a timeframe associated with it. The other is a ‘for information’ message, which is for the GP to inspect and file against the patients record.<dd>

  <dt><a name="renderedpem">Rendered PEM</a></dt>
  <dd>Rendered PEM means 'Rendered Post Event Message' which refers to a CDA document which has been converted from XML format (designed for processing by software) to a human-readable format such as PDF or HTML.<br><br>

  <a href="../technical_faq#renderedpem">Full Explanation</a>
  <dd>

  <dt><a name="trud">TRUD</a></dt>
  <dd>TRUD stands for <b>T</b>erminology <b>R</b>eference data <b>U</b>pdate <b>D</b>istribution site and is a website that the Health and Social Care Information Centre uses to distribute specifications and resources to be used for NHS Information Technology e.g.
  <br><br>
  <ul>
  <li>Messaging Specifications</li>
  <li>Clinical Code Lists</li>
  <li>Accreditation Guidance....</li>
  </ul>
  You can access the TRUD Website here: <a href="https://isd.hscic.gov.uk/">https://isd.hscic.gov.uk</a>
  <dd>

</dl>
