# Introduction

MolecularMatch is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Customers.  As a provider of a compliant cloud-based solution for enabiling patient's to take control of their data and use that to improve their care, MolecularMatch strives to maintain compliance, proactively address information security issues, and mitigate the risk of data loss.  MolecularMatch assures known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by MolecularMatch to maintain compliance and assure the proper protections of web, infrastructure, and administrative components of the solution used to store, process, and transmit ePHI.

MolecularMatch provides secure and compliant clinical trial and drug-based information resources deliveried through cloud-based software. 

## Compliance Inheritance

MolecularMatch provides a web application enabling patients, physicians, and principal investigators to search for and manage the enrollment process around clinical trials.  Principal Investigators of these clinical trials may where allowed have the ability to review de-identified information about patients and express an interest in evaluating them for a fit with the clinical trial.  MolecularMatch has been through a HIPAA compliance audit by a 3rd party to validate and map organizational policies and technical settings to HIPAA rules (where applicable). 

MolecularMatch sometimes signs business associate agreements (BAAs) with Covered Entities (CEs). These BAAs outline the obligations of both MolecularMatch and the Covered Entity, as well as liability in the case of a breach as defined by the HIPAA standard. When providing a web application and other related services that are part of the technology requirements that exist in HIPAA and HITRUST, as well as future compliance frameworks, MolecularMatch manages their responsibilities for  compliance. 

MolecularMatch does use third party, subcontractors to aid in managing some of the compliance and risk.  Currently, they are Catalyze.io, a secure, HIPAA compliant cloud solution for hosting and managing web and data servers.  As such, those aspects that Catalyze.io manages for MolecularMatch are inherited by Customers, and Catalyze.io assumes the risk associated with those aspects of compliance. In doing so, Catalyze.io helps MolecularMatch achieve and maintain compliance, as well as mitigates MolecularMatch's risk.

Below are mappings of HIPAA Rules to MolecularMatch controls and a mapping of what Rules are managed by Catalyze.io.

## MolecularMatch Organizational Concepts

The physical infrastructure environment is hosted by Catalyze.io via [Rackspace](http://broadcast.rackspace.com/downloads/pdfs/RackspaceSecurityApproach.pdf) and Amazon Web Services (AWS). The network components and supporting network infrastructure is contained within AWS and Rackspace infrastructure and managed by Rackspace and AWS. Neither MolecularMatch nor Catalyze.io have physical access into the network components. The Catalyze.io environment consists of Cisco firewalls, Apache web servers, Dropwizard Java application servers, Percona and Riak database servers, Logstash logging servers, Linux Ubuntu monitoring servers, Puppet access control server, OSSEC IDS services, Docker containers, Linux CentOS bastion host, and developer tools servers running on Linux Ubuntu.  In addition, MolecularMatch uses a node.js web application framework and MongoDB for storage of all data.  These are hosted within the Catalyze.io infrastructure mentioned above.

Within the Catalyze.io Platform, both on Rackspace and AWS, all data transmission is encrypted and all hard drives are encrypted so data at rest is also encrypted; this applies to all servers - those hosting Docker containers, databases, APIs, log servers, etc. Both MolecularMatch and Catalyze.io always assume all data *may* contain ePHI, even though our Risk Assessment does not indicate this is the case, and thus provide proactive protections based on that assumption.

MolecularMatch restricts, secures, and assures the privacy of all ePHI data at the Application Level, as this is not under the control or purview of Catalyze.io.  This is done using appropriate access controls, monitoring, and security frameworks.  Specifically all data is encrypted in transit using SSL.  Users are managed in the application server and no user regardless of role can see another user's ePHI.  

There is data and network segmentation in place.  This is currently managed by Catalyze.io.  Load balancers segment data, while firewalls route traffic to private subnets.  Creating dedicated Virtual Private Clouds.  As a result of segmentation strategies employed by Catalyze.io, they have effectively create RFC 1918, or dedicated, private segmented and separated networks and IP spaces, for the MolecularMatch web application. 

Additionally, Catalyze.io uses IPtables on each server for logical segmentation. The IPtables are configured to restrict access to only justified ports and protocols. Catalyze.io has implemented strict logical access controls so that only authorized personnel are given access to the internal management servers. The environment is configured so that data is transmitted from the load balancers to the application servers over an SSL encrypted session.

Once the data is received from the application server, a series of Application Programming Interface (API) calls is made to the database servers where the potential ePHI resides. The ePHI is separated through programming logic built, so that access to one database server will not allow access to the full ePHI spectrum. 

Only the web application servers are public facing and accessible via the Internet. The database servers, where any potential ePHI would reside, are located on the private, internal network and can only be accessed directly over an SSH connection through the bastion host. The access to the internal database is restricted to a limited number of personnel and strictly controlled to only those personnel with a business justified reason. Remote access to the internal servers is not accessible except through the load balancers and bastion host.

All updates to the web application and data servers are tested end-to-end for usability, security, and impact prior to deployment to production.

## Version Control

Policies were last updated October 29th, 2014.