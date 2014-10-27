
# Auditing Policy

MolecularMatch will audit access and activity of electronic protected health information (ePHI) applications and systems in order to ensure compliance. The Security Rule requires healthcare organizations to implement reasonable hardware, software, and/or procedural mechanisms that record and examine activity in information systems that contain or use ePHI. Audit activities may be limited by application, system, and/or network auditing capabilities and resources. We shall make reasonable and good-faith efforts to safeguard information privacy and security through a well-thought-out approach to auditing that is consistent with available resources.

This policy, and associated procedures for auditing and monitoring, has been sub-contracted in part to a third-party, HIPAA compliant vendor.  We have verified that their policies and procedures meet or exceed our standards and those of HIPAA and the HITRUST Common Security Framework.  As such, we have assurances that monitoring and auditing systems are available on all systems hosted by our sub-contractor.  Proof of such due diligence is kept by the Security Officer.
  
Auditing is an important part of the day-to-day operations of our Platform as a Service (PaaS), third-party provider. It is our policy to review and monitor audting and logging of activity on the web application, as well as on the production web and data servers.  The PaaS vendor performs their own appropriate auditing and logging to the integrity of the hosting environment.  

It is our policy to safeguard the confidentiality, integrity, and availability of applications, systems, and networks. To ensure that appropriate safeguards are in place and effective, we shall audit access and activity to detect, report, and guard against:

* Breaches in confidentiality and security of patient protected health information;
* Performance problems and flaws in applications;
* Improper alteration or destruction of ePHI;

The PaaS vendor also supports this aim by detecting, reporting, and guarding against:

* Network vulnerabilities and intrusions;
* Out of date software and/or software known to have vulnerabilities.
* Breaches in confidentiality and security of patient protected health information;
* Performance problems and flaws in applications;
* Improper alteration or destruction of ePHI;



## Applicable Standards from the HITRUST Common Security Framework

* 0.a Information Security Management Program
* 01.a Access Control Policy
* 01.b User Registration
* 01.c Privilege Management
* 09.aa Audit Logging
* 09.ac Protection of Log Information
* 09.ab - Monitoring System Use
* 06.e - Prevention of Misuse of Information

## Applicable Standards from the HIPAA Security Rule

* 45 CFR ¬ß 164.308(a)(1)(ii)(D) - Information System Activity Review
* 45 CFR ¬ß 164.308(a)(5)(ii)(B) & (C) - Protection from Malicious Software & Log-in Monitoring
* 45 CFR ¬ß 164.308(a)(2) - HIPAA Security Rule Periodic Evaluation
* 45 CFR ¬ß 164.312(b) - Audit Controls
* 45 CFR ¬ß 164.312(c)(2) - Mechanism to Authenticate ePHI
* 45 CFR ¬ß 164.312(e)(2)(i) - Integrity Controls

# Auditing Policies

1. Responsibility for auditing information system access and activity is assigned to the Security Officer. The Security Officer shall:
	* Assign the task of generating reports for audit activities to the workforce member responsible for the application, system, or network;
	* Assign the task of reviewing the audit reports to the workforce member responsible for the application, system, or network, the Privacy Officer, or any other individual determined to be appropriate for the task;
	* Organize and provide oversight to a team structure charged with audit compliance activities (e.g., parameters, frequency, sample sizes, report formats, evaluation, follow-up, etc.).
2. The auditing processes shall address access and activity at the following levels listed below. In the case of PaaS Vendor, System and Netowrk level auditing is the responsibility of the PaaS Vendor as per BAA and Service Agreement.  PaaS vendor provides software to aggregate and view User and Application logs, but the log data collected is our responsibility. Auditing processes may address date and time of each log-on attempt, date and time of each log-off attempt, devices used, functions performed, etc.
	* User: User level audit trails generally monitor and log all commands directly initiated by the user, all identification and authentication attempts, and data and services accessed.
	* Application: Application level audit trails generally monitor and log all user activities, including data accessed and modified and specific actions.
	* System: System level audit trails generally monitor and log user activities, applications accessed, and other system defined specific actions. **PaaS vendor responsibility.**
	* Network: Network level audit trails generally monitor information on what is operating, penetrations, and vulnerabilities.  **PaaS vendor responsibility.**
3. We shall log all incoming and outgoing traffic to into and out of its environment. This includes all successful and failed attempts at data access and editing. Data associated with this data will include origin, destination, time, and other relevant details that are available to Catalyze.
4. PaaS Vendor:
	1. Utilizes OSSEC to scan all systems for malicious and unauthorized software every 2 hours and at reboot of systems. Alerts from OSSEC are sent to Kibana, the centralized logging service that we use.
	2. Uses Nagios to monitor systems in its environment. 
	3. Treats its Developer Portal as a Platform Add-on and, as such, it logs all activity associated with Developer Portal Access.
	4. Uses OSSEC to monitor the integrity of log files by utilizing OSSEC System Integrity Checking capabilities.
	5. Shall identify “trigger events” or criteria that raise awareness of questionable conditions of viewing of confidential information. *(See Listing of Potential Trigger Events below)*
	6. Utilize OSSEC log correlation functionality to proactively identify and enable alerts based on log data.
	7. Use auditing tools that are designed to detect network vulnerabilities and intrusions.  
10. Logs are reviewed weekly by Security Officer. 
12. The process for review of audit logs, trails, and reports shall include:
	* Description of the activity as well as rationale for performing the audit.
	* Identification of which workforce members will be responsible for review.  Workforce members shall not review audit logs that pertain to their own system activity.
	* Frequency of the auditing process.
	* Determination of significant events requiring further review and follow-up.
	* Identification of appropriate reporting channels for audit results and required follow-up.
13. Vulnerability testing software may be used to probe the network to identify what is running (e.g., operating system or product versions in place), whether publicly-known vulnerabilities have been corrected, and evaluate whether the system can withstand attacks aimed at circumventing security controls.
	* Testing may be carried out internally or provided through an external third-party vendor. Whenever possible, a third party auditing vendor should not be providing the organization IT oversight services (e.g., vendors providing IT services should not be auditing their own services - separation of duties).
	* Testing shall be done on a routine basis, currently monthly.
14. Software patches and updates will be applied in the following manner.  In the case of routine updates, they will be applied after thorough testing. In the case of updates to correct known vulnerabilities, priority will be given to testing to speed the time to production. Critical security patches are applied within 30 days from testing and all patches are applied within 90 days after testing.
	* We will perform updates Application and Database versions, although the PaaS Vendor may notify and recommend updates to our systems as well.
	*  **PaaS Vendor** is responsibile for Server, Network, and Operating Systems.  

## Audit Requests

1. A request may be made for an audit for a specific cause. The request may come from a variety of sources including, but not limited to, Privacy Officer, Security Officer, Customer, Partner, or an Application owner or application user.
2. A request for an audit for specific cause must include time frame, frequency, and nature of the request. The request must be reviewed and approved by either the Privacy or Security Officer.
3. A request for an audit must be approved by either the Privacy Officer or Security Officer before proceeding. Under no circumstances shall detailed audit information be shared with parties without proper permissions and access to see such data.
	* Only de-identified information shall be shared with Customer or Partner regarding the results of the investigative audit process. This information will be communicated to the appropriate personnel by the Privacy Officer or designee. Prior to communicating with Customer or Partner regarding an audit, it is recommended that risk management and/or legal counsel is sought.

## Review and Reporting of Audit Findings

1. Audit information that is routinely gathered must be reviewed in a timely manner, currently monthly, by the responsible workforce member(s).
2. The reporting process shall allow for meaningful communication of the audit findings to those workforce members, Customers, or Partners requesting the audit.
	* Significant findings shall be reported immediately in a written format. Our security incident response form may be utilized to report a single event.
	* Routine findings shall be reported to the sponsoring leadership structure in a written report format.
3. Reports of audit results shall be limited to internal use on a minimum necessary/need-to-know basis. Audit results shall not be disclosed externally without administrative and legal counsel approval.
4. Security audits constitute an internal, confidential monitoring practice that may be included in performance improvement activities and reporting. Care shall be taken to ensure that the results of the audits are disclosed to administrative level oversight structures only and that information which may further expose organizational risk is shared with extreme caution. Generic security audit information may be included in organizational reports (individually-identifiable ePHI shall not be included in the reports).
5. Whenever indicated through evaluation and reporting, appropriate corrective actions must be undertaken. These actions shall be documented and shared with the responsible workforce members, Customers, and/or Partners.

## Audit Log Security Controls and Backup

4. Audit logs shall be protected from unauthorized access or modification, so the information they contain will be made available only if needed to evaluate a security incident or for routine audit activities as outlined in this policy.
5. All audit logs are encrypted in transit and at rest to control access to the content of the logs. 
6. Audit logs shall be stored on a separate system to minimize the impact auditing may have on the privacy system and to prevent access to audit trails by those with system administrator privileges. This is done to apply the security principle of “separation of duties” to protect audit trails from hackers.

## Workforce Training, Education, Awareness, and Responsibilities

1. Workforce members are provided training, education, and awareness on safeguarding the privacy and security of business and ePHI. Our commitment to auditing access and activity of the information applications, systems, and networks is communicated through new employee orientation, ongoing training opportunities and events, and applicable policies. Workforce members are made aware of responsibilities with regard to privacy and security of information as well as applicable sanctions/corrective disciplinary actions should the auditing process detect a workforce member’s failure to comply with organizational policies.

## External Audits of Information Access and Activity

1. Prior to contracting with an external audit firm, we shall:
	* Outline the audit responsibility, authority, and accountability;
	* Choose an audit firm that is independent of other organizational operations;
	* Ensure technical competence of the audit firm staff;
	* Require the audit firm’s adherence to applicable codes of professional ethics;
	* Obtain a signed HIPAA business associate agreement;
	* Assign organizational responsibility for supervision of the external audit firm.

## Retention of Audit Data

1. Audit logs shall be maintained based on organizational needs. There is no standard or law addressing the retention of audit log/trail information. Retention of this information shall be based on:
	* Organizational history and experience.
	* Available storage space.
2. Reports summarizing audit activities shall be retained for a period of six years.
3. Log data is currently retained and readily accessible for a 1-month period. Beyond that, log data is available via cold backup. 

## Potential Trigger Events

* High risk or problem prone incidents or events.
* Business associate, customer, or partner complaints.
* Known security vulnerabilities.
* Atypical patterns of activity.
* Failed authentication attempts.
* Remote access use and activity.
* Activity post termination.
* Random audits.
