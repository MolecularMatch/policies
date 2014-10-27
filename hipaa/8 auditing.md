#Auditing Policy
Catalyze shall audit access and activity of electronic protected health information (ePHI) applications and systems in order to ensure compliance. The Security Rule requires healthcare organizations to implement reasonable hardware, software, and/or procedural mechanisms that record and examine activity in information systems that contain or use ePHI.  Audit activities may be limited by application, system, and/or network auditing capabilities and resources. Catalyze shall make reasonable and good-faith efforts to safeguard information privacy and security through a well-thought-out approach to auditing that is consistent with available resources.

It is the policy of Catalyze to safeguard the confidentiality, integrity, and availability of applications, systems, and networks.  To ensure that appropriate safeguards are in place and effective, Catalyze shall audit access and activity to detect, report, and guard against:

* Network vulnerabilities and intrusions;
* Breaches in confidentiality and security of patient protected health information;
* Performance problems and flaws in applications;
* Improper alteration or destruction of ePHI;
* Out of date software and/or software known to have vulnerabilities.

##Applicable Standards from the HITRUST Common Security Framework

* 0.a Information Security Management Program
* 01.a Access Control Policy
* 01.b User Registration
* 01.c Privilege Management
* 09.aa Audit Logging
* 09.ac Protection of Log Information
* 09.ab - Monitoring System Use
* 06.e - Prevention of Misuse of Information

##Applicable Standards from the HIPAA Security Rule

* 45 CFR § 164.308(a)(1)(ii)(D)  – Information System Activity Review
* 45 CFR § 164.308(a)(5)(ii)(B) & (C) – Protection from Malicious Software & Log-in Monitoring
* 45 CFR § 164.308(a)(2) – HIPAA Security Rule Periodic Evaluation
* 45 CFR § 164.312(b) –Audit Controls
* 45 CFR § 164.312(c)(2) – Mechanism to Authenticate ePHI
* 45 CFR § 164.312(e)(2)(i) – Integrity Controls

##Auditing Policies
1. Responsibility for auditing information system access and activity is assigned to Catalyze’s Security Officer.  The Security Officer shall:
	2. Assign the task of generating reports for audit activities to the workforce member responsible for the application, system, or network;
	3. Assign the task of reviewing the audit reports to the workforce member responsible for the application, system, or network, the Privacy Officer, or any other individual determined to be appropriate for the task;
	4. Organize and provide oversight to a team structure charged with audit compliance activities (e.g., parameters, frequency, sample sizes, report formats, evaluation, follow-up, etc.).

2.	Catalyze’s auditing processes shall address access and activity at the following levels listed below. In the case of PaaS Custoners, Application and User level auditing is the responsibility of the Customer; Catalyze provides software to aggregate and view User and Application logs, but the log data collected is the responsibility of the PaaS Customer. Auditing processes may address date and time of each log-on attempt, date and time of each log-off attempt, devices used, functions performed, etc.
	3. User: User level audit trails generally monitor and log all commands directly initiated by the user, all identification and authentication attempts, and data and services accessed.
	4. Application: Application level audit trails generally monitor and log all user activities, including data accessed and modified and specific actions.
	5. System:  System level audit trails generally monitor and log user activities, applications accessed, and other system defined specific actions. Catalyze utilizes file system monitoring from OSSEC to assure the integrity of file system data.
	6. Network:  Network level audit trails generally monitor information on what is operating, penetrations, and vulnerabilities.

3. Catalyze shall log all incoming and outgoing traffic to into and out of its environment. This includes all successful and failed attempts at data access and editing. Data associated with this data will include origin, destination, time, and other relevant details that are available to Catalyze.

4. Catalyze treats its Developer Portal as a Platform Add-on and, as such, it logs all activity associated with Developer Portal Access.

5. Catalyze uses OSSEC to monitor the integrity of log files by utilizing OSSEC System Integrity Checking capabilities.

5. In addition to trigger events, Catalyze utilizes OSSEC log correlation functionality to proactively identify and enable alerts based on log data.
	* Scanning tools and devices;
	* Password cracking utilities;
	* Network “sniffers.”
	* Passive and active intrusion detection systems.
	1. Description of the activity as well as rationale for performing the audit.
	2. Identification of which Catalyze workforce members will be responsible for review (workforce members shall not review audit logs that pertain to their own system activity).
	3. Frequency of the auditing process.
	4. Determination of significant events requiring further review and follow-up.
	5. Identification of appropriate reporting channels for audit results and required follow-up.
	* Testing may be carried out internally or provided through an external third-party vendor.  Whenever possible, a third party auditing vendor should not be providing the organization IT oversight services (e.g., vendors providing IT services should not be auditing their own services – separation of duties).
	* Testing shall be done on a routine basis, currently monthly.

8. Software patches and updates will be applied to all systems in a timely manner. In the case of routine updates, they will be applied after thorough testing. In the case of updates to correct known vulnerabilities, priority will be given to testing to speed the time to production.
	* In the case of PaaS Customers, updates to Application and Database versions are the responsibilty of Customers, though Catalyze will, at it's own discretion, notify and recommend updates to customer systems.

	
##Audit Requests
	* Should the audit disclose that a workforce member has accessed ePHI inappropriately, the minimum necessary/least privileged information shall be shared with Catalyze’s Security Officer to determine appropriate sanction/ corrective disciplinary action.
	* Only de-identified information shall be shared with Customer or Partner regarding the results of the investigative audit process. This information will be communicated to the appropriate personnel by Catalyze’s Privacy Officer or designee.  Prior to communicating with customers and partners regarding an audit, it is recommended that Catalyze consider seeking risk management and/or legal counsel.

##Review and Reporting of Audit Findings
	* Significant findings shall be reported immediately in a written format. Catalyze’s security incident response form may be utilized to report a single event.
	* Routine findings shall be reported to the sponsoring leadership structure in a written report format.

##Auditing Customer and Partner Activity

##Audit Log Security Controls and Backup 

22. For PaaS Customers choosing to use Catalyze logging services, log data will be separated from the log data of other Catalyze Customers.

23. Catalyze Customers are provided with necessary information to understand Catalyze auditing capabilities, and PaaS Customers can choose the level of logging and auditing that Catalyze will implement on their behalf.

##External Audits of Information Access and Activity
	* Outline the audit responsibility, authority, and accountability;
	* Choose an audit firm that is independent of other organizational operations;
	* Ensure technical competence of the audit firm staff;
	* Require the audit firm’s adherence to applicable codes of professional ethics;
	* Obtain a signed HIPAA business associate agreement;
	* Assign organizational responsibility for supervision of the external audit firm.
23. Log data is currently retained and readily accessible for a 1 month period. Beyond that, log data is available via cold backup. 

24. For Paas Customers, they choose the length of backup retention and availability that Catalyze will implement and enforce.

##Potential Trigger Events
* Known security vulnerabilities.
* Atypical patterns of activity.
* Failed authentication attempts.
* Remote access use and activity.
* Activity post termination.
* Random audits.