Catalyze is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it creates, receives, maintains, and/or transmits on behalf of its customers. As providers of compliant infrastructure used by health technology vendors, developers, designers, agencies, custom development  shops, and enterprises, Catalyze strives to maintain compliance, proactively address information security, mitigate risk for its customers, and assure known breaches are completely and effectively communicated. The following documents address core policies used by Catalyze to maintain compliance and assure the proper protections of infrastructure used to store, process, and trasmit ePHI for Catalyze customers.


Catalyze, Inc (“Catalyze”) provides secure and compliant cloud-based software. This hosted software falls into two broad offerings: 1) **Platform as a Service (Paas)** and 2) **Platform Add-ons**.

Platform as a Service
==================


Platform Add-ons
==================

partner and internal


#Key Definitions

* *Application*: An application hosted by Catalyze, either maintained and created by Catalyze, or maintaiend and created by a Customer or Partner.

* *Application Level*: Controls and security associated with an Application. In the case of PaaS Customers, Catalzye does not have access to and cannot assure compliance with security standards and policies at the Application Level.

* *Audit*:  Internal process of reviewing information system access and activity (e.g., log-ins, file accesses, and security incidents).  An audit may be done as a periodic event, as a result of a patient complaint, or suspicion of employee wrongdoing.

* *Audit Controls*:  Technical mechanisms that track and record computer/system activities.* *Audit Logs*:  Encrypted records of activity maintained by the system which provide:  1) date and time of activity; 2) origin of activity (app); 3) identification of user doing activity; and 4) data accessed as part of activity.

* *Access*:   Means the ability or the means necessary to read, write, modify, or communicate data/ information or otherwise use any system resource.

* *BaaS*: Backend-as-a-Service. A set of APIs, and associated SDKs, for rapid mobile and web application development. APIs offer the ability to create users, do authentication, store data, and store files.

* *Backup Service*:* *Breach*:  Means the acquisition, access, use, or disclosure of protected health information (PHI) in a manner not permitted under the Privacy Rule which compromises the security or privacy of the PHI.  For purpose of this definition, “compromises the security or privacy of the PHI” means poses a significant risk of financial, reputational, or other harm to the individual.  A use or disclosure of PHI that does not include the identifiers listed at §164.514(e)(2), limited data set, date of birth, and zip code does not compromise the security or privacy of the PHI. Breach excludes:

	1. Any unintentional acquisition, access or use of PHI by a workforce member or person acting under the authority of a Covered Entity (CE) or Business Associate (BA) if such acquisition, access, or use was made in good faith and within the scope of authority and does not result in further use or disclosure in a manner not permitted under the Privacy Rule.
	2. Any inadvertent disclosure by a person who is authorized to access PHI at a CE or BA to another person authorized to access PHI at the same CE or BA, or organized health care arrangement in which the CE participates, and the information received as a result of such disclosure is not further used or disclosed in a manner not permitted under the Privacy Rule.
	3. A disclosure of PHI where a CE or BA has a good faith belief that an unauthorized person to whom the disclosure was made would not reasonably have been able to retain such information. * *Business Associate*: a person or entity that performs certain functions or activities that involve the use or disclosure of protected health information on behalf of, or provides services to, a covered entity. * *Covered Entity*:  A health plan, health care clearinghouse, or a healthcare provider who transmits any health information in electronic form. 

* *De-identification*:

* *Disaster Recovery*:* *Disclosure*:  Disclosure means the release, transfer, provision of, access to, or divulging in any other manner of information outside the entity holding the information.

* *Customers*:

* *Electronic Protected Health Information (ePHI)*:  Any individually identifiable health information protected by HIPAA that is transmitted by, processed in some way, or stored in electronic media. 

* *Environment*:'

* *Health and Human Services (HHS)*:

* *Individually Identifiable Health Information*:  That information that is a subset of health information, including demographic information collected from an individual, and is created or received by a health care provider, health plan, employer, or health care clearinghouse; and relates to the past, present, or future physical or mental health or condition of an individual; the provision of health care to an individual; or the past, present, or future payment for the provision of health care to an individual; and identifies the individual; or with respect to which there is a reasonable basis to believe  the information can be used to identify the individual. 

* *Intrusion Detection System (IDS)*: A software tool use to automatically detect and notify in the event of possible unauthorized network and/or system access. * *Law Enforcement Official*:  Any officer or employee of an agency or authority of the United States, a State, a territory, a political subdivision of a State or territory, or an Indian tribe, who is empowered by law to investigate or conduct an official inquiry into a potential violation of law; or prosecute or otherwise conduct a criminal, civil, or administrative proceeding arising from an alleged violation of law.

* *Logging Service*:

* *Messaging*: API-based services to deliver and receive SMS messages.* *Organization*:  For the purposes of this policy, the term “organization” shall mean Catalyze.

* *Partner*:

* *Platform*:* *Protected Health Information (PHI)*:  Individually identifiable health information that is created by or received by the organization, including demographic information, that identifies an individual, or provides a reasonable basis to believe the information can be used to identify an individual, and relates to:  	* Past, present or future physical or mental health or condition of an individual.
	* The provision of health care to an individual.
	* The past, present, or future payment for the provision of health care to an individual.* *Sanitization*:  Removal or the act of overwriting data to a point of preventing the recovery of the data on the device or media that is being sanitized. Sanitization is typically done before re-issuing a device or media, donating equipment that contained sensitive information or returning leased equipment to the lending company.* *Trigger Event*:  Activities that may be indicative of a security breach that require further investigation (See Appendix).

* *Unsecured Protected Health Information*:   Protected health information (PHI) that is not rendered unusable, unreadable, or indecipherable to unauthorized individuals through the use of technology or methodology specified by the Secretary in the guidance issued under section 13402(h)(2) of Pub. L.111-5 on the HHS website.
	1. Electronic PHI has been encrypted as specified in the HIPAA Security rule by the use of an algorithmic process to transform data into a form in which there is a low probability of assigning meaning without the use of a confidential process or key and such confidential process or key that might enable decryption has not been breached.  To avoid a breach of the confidential process or key, these decryption tools should be stored on a device or at a location separate from the data they are used to encrypt or decrypt.  The following encryption processes meet this standard.
		* Valid encryption processes for data at rest (i.e. data that resides in databases, file systems and other structured storage systems) are consistent with NIST Special Publication 800-111, Guide to Storage Encryption Technologies for End User Devices.
		* Valid encryption processes for data in motion (i.e. data that is moving through a network, including wireless transmission) are those that comply, as appropriate, with NIST Special Publications 800-52, Guidelines for the Selection and Use of Transport Layer Security (TLS) 	Implementations; 800-77, Guide to IPsec VPNs; or 800-113, Guide to SSL VPNs, and may include others which are Federal Information Processing Standards FIPS 140-2 validated.
	2.  The media on which the PHI is stored or recorded has been destroyed in the following ways:
		*  Paper, film, or other hard copy media have been shredded or destroyed such that the PHI cannot be read or otherwise cannot be reconstructed.  Redaction is specifically excluded as a means of data destruction.
		*  Electronic media have been cleared, purged, or destroyed consistent with NIST 	Special Publications 800-88, Guidelines for Media Sanitization, such that the PHI cannot be retrieved.* *Workforce*:  Means employees, volunteers, trainees, and other persons whose conduct, in the performance of work for a covered entity, is under the direct control of such entity, whether or not they are paid by the covered entity. 

* *Restricted Area*: Those areas of the building(s) where protected health information and/or sensitive organizational information is stored, utilized, or accessible at any time. * *Role*:  The category or class of person or persons doing a type of job, defined by a set of similar or identical responsibilities.* *Unrestricted Area*: those areas of the building(s) where protected health information and/or sensitive organizational information is not stored or is not utilized or is not accessible there on a regular basis.* *Vendors*: persons from other organizations marketing or selling products or services, or providing services to Catalyze. * *Workstation*:  An electronic computing device, such as a laptop or desktop computer, or any other device that performs similar functions, used to create, receive, maintain, or transmit ePHI.  Workstation devices may include, but are not limited to: laptop or desktop computers, personal digital assistants (PDAs), tablet PCs, and other handheld devices.  For the purposes of this policy, “workstation” also includes the combination of hardware, operating system, application software, and network connection.* *Event*:  An event is defined as an occurrence that does not constitute a serious adverse effect on Catalyze, its operations, or its Customers, though it may be less than optimal.  Examples of events include, but are not limited to:
	*  A hard drive malfunction that requires replacement;
	*  Systems become unavailable due to power outage that is non-hostile in nature, with redundancy to assure ongoing availability of data;
	*  Accidental lockout of an account due to incorrectly entering a password multiple times.
* *Indication*:  A sign that an Incident may have occurred or may be occurring at the present time.  Examples of indications include:
	* The network intrusion detection sensor alerts when a known exploit occurs against an FTP server.  Intrusion detection is generally reactive, looking only for footprints of known attacks.  It is important to note that many IDS “hits” are also false positives and are neither an event nor an incident;
	* The antivirus software alerts when it detects that a host is infected with a worm;
	* Users complain of slow access to hosts on the Internet;
	* The system administrator sees a filename with unusual characteristics;
	* Automated alerts of activity from log monitors like OSSEC;
	* An alert from OSSEC about file system integrity issues.
* *Precursor*:  A sign that an Incident may occur in the future.  Examples of precursors include:
	* Suspicious network and host-based IDS events/attacks;
	* Alerts as a result of detecting malicious code at the network and host levels;
	* Alerts from file integrity checking software;
	* Audit log alerts.* *Security Incident* (or just Incident):  A security incident is an occurrence that exercises a significant adverse effect on people, process, technology, or data.  Security incidents include, but are not limited to: 
	* A system or network breach accomplished by an internal or external entity; this breach can be inadvertent or malicious;
	* Unauthorized disclosure;
	* Unauthorized change or destruction of ePHI (i.e. delete dictation, data alterations not following Catalyze’s procedures);
	* Denial of service not attributable to identifiable physical, environmental, human or technology causes;
	* Disaster or enacted threat to business continuity;
	* Information Security Incident:  A violation or imminent threat of violation of information security policies, acceptable use policies, or standard security practices.  Examples of information security incidents may include, but are not limited to, the following:
	* Denial of Service:  An attack that prevents or impairs the authorized use of networks, systems, or applications by exhausting resources;
	* Malicious Code:  A virus, worm, Trojan horse, or other code-based malicious entity that infects a host;
	* Unauthorized Access/System Hijacking:  A person gains logical or physical access without permission to a network, system, application, data, or other resource.  Hijacking occurs when an attacker takes control of network devices or workstations;
	* Inappropriate Usage:  A person violates acceptable computing use policies;
	* Other examples of observable information security incidents may include, but are not limited to:
		* Use of another person’s individual password and/or account to login to a system;
		* Failure to protect passwords and/or access codes (e.g., posting passwords on equipment);
		* Installation of unauthorized software;
		* Terminated workforce member accessing applications, systems, or network.#Catalyze Organizational Concepts

The physical infrastructure environment is hosted at Rackspace and Amazon Web Services (AWS). The network components and supporting network infrastructure is contained within AWS and Rackspace infrastructure and managed by Rackspace and AWS. Catalyze does not have physical access into the network components. The Catalyze environment consists of Cisco firewalls, Apache web servers, Dropwizard Java application servers, Percona and Riak database servers, Logstash logging servers, Linux Ubuntu monitoring servers, Puppet access control server, OSSEC IDS services, Docker containers, Linux CentOS bastion host, and developer tools servers running on Linux Ubuntu.

Within the Catalyze Platform, both on Rackspace and AWS, all data transmission is encrypted and all hard drives are encrypted so data at rest is also encrypted; this applies to all servers - those hosting Docker containes, databases, APIs, log servers, etc. Catalyze assumes all data *may* contain ePHI, even though our Risk Assessment does not indicate this is the case, and provides appropriate protections based on that assumption.

In the case of PaaS Customers, it is the responsilibity of the Customer to restrict, secure, and assure the privacy of all ePHI data at the Application Level, as this is not under the control or perview of Catalyze.There is data and network segmentation in place but differently implemented on Rackspace and AWS versions of the Catalyze Platform.

* With Rackspace, hosted load balancers segment data and traffic while Cisco firewalls route traffic to private subnets for each PaaS Customer and for Platform Add-ons.
* With AWS, hosted load balancers segment data across dedicated Virtual Privare Clouds for each PaaS Customer and for Platform Add-ons.

The result of segmentation strategies employed by Catalyze effectively create RFC 1918, or dedicated, private segmented and separated networks and IP spaces, for each PaaS Customer and for Platform Add-ons. 

Additionally, IPtables is used on each each server for logical segmentation. The IPtables are configured to restrict access to only justified ports and protocols. Catalyze has implemented strict logical access controls so that only authorized personnel are given access to the internal management servers. The environment is configured so that data is transmitted from the load balancers to the application servers over an SSL encrypted session.

In the case of Platform Add-ons, once the data is received from the application server, a series of Application Programming Interface (API) calls is made to the database servers where the ePHI resides. The ePHI is separated into Riak and Percona databases through programming logic built, so that access to one database server will not present you with the full ePHI spectrum. The bastion host, Apache web server, Dropwizard application servers are externally facing and accessible via the Internet. The database servers, where the ePHI resides, are located on the internal Catalyze network and can only be accessed directly over an SSH connection through the bastion host. The access to the internal database is restricted to a limited number of personnel and strictly controlled to only those personnel with a business justified reason. Remote access to the internal servers is not accessible except through the load balancers and bastion host.#Version Control

Policies were last updated March 31st, 2014.