![Server General logo](https://www.servergeneral.com/wp-content/uploads/mediapress/server-general-logo.png)
 
### Summary ###
*Server General KMS for MySQL* is a key management service for customers who want to use MySQL TDE to encrypt their data, but do not want to build or manage a complicated, expensive and time-consuming in-house key management system. 
 
With *Server General KMS for MySQL*, you can focus on developing your business applications while we securely manage your MySQL master encryption keys to meet your compliance requirements. *Server General KMS for MySQL* also enables you to store your encryption keys on-premises in a secure, managed key locker appliance, or in our secure cloud key locker management service (both sold separately). We protect your MySQL database server on any cloud platform or in your own data center. Customers use our service to comply with the security requirements of the HIPAA Act and the PCI DSS mandates.
 
### Description ###
In 2016, Oracle added Transparent Data Encryption (TDE) feature to the MySQL server. With this new functionality, database administrators can now encrypt sensitive information stored in their MySQL database servers to ensure privacy and prevent data breaches. Moreover, the functionality is available for free in the MySQL Community edition. However, both the Community and the Enterprise edition lack effective key management. Oracle recommends *Oracle Data Vault* (or any other KMIP compliant key locker) for managing MySQL master encryption keys. However, the cost of such a solution can run into tens of thousands of dollars - a small fortune for many small-to-medium-sized businesses.
 
*Server General KMS for MySQL* is a key management service for customers who want to use the embedded MySQL TDE functionality, but don’t want to take on the arduous task of building and managing an expensive key management system. The service enables customers to offload their key management responsibilities to us. Our global key management infrastructure is managed by our security experts on 24x7x365 basis. We ensure that the encryption keys are stored securely and are available to authorized individuals when needed. Our key management procedures are designed to meet or exceed data compliance requirements of various regulations including that of the HIPAA/HITECH Act. It usually takes less than 30 minutes to install and configure our service. The service is ideal for small-to-medium-sized businesses.
 
*Server General KMS for MySQL* is built on top of our secure platform, Server General. The core components of our platform are a data encryption engine, a key management engine, an access control engine, and a reporting engine. Each component performs a critical function in securing the MySQL Master Key (MMK).
 
 
This diagram illustrates how *Server General KMS for MySQL* works.
 
![*Server General KMS for MySQL* Architecture](https://www.servergeneral.com/wp-content/uploads/mediapress/how_does_it_work_kms.png)
 
### Additional Information ###
For more details on *Server General KMS for MySQL* architecture, please visit the [Server General Technology page](https://www.servergeneral.com/products/kms/mysql/). 
 
### Deployment Process ###
This Runner job performs the following steps:
 
1. Installs a Server General Agent on your MySQL server deployed within CenturyLink Cloud account and initiates a monthly recurring subscription.
2. Gets hold of basic customer information in order to generate a customer record.
3. Initializes a system user - “sgadmin” in order to manage the *Server General KMS for MySQL* installation.
4. Acquires a Server General Agent subscription license and applies it to your server. This step also provisions a cloud key locker account.
5. Notifies the Server General on-boarding team who will contact you within 1 business day.
 
### Prerequisite(s) ###
* Access to the CenturyLink Cloud as an authorized user.
* Target server operating system must be one of the following: Ubuntu 14.04, Ubuntu 16.04, Debian 7, Debian 8, RHEL 6.x, CentOS 6.x.
* MySQL Server version 5.7.12 or greater on the target server.
* The designated contact information.
 
 
### Post-requisite(s) ###
* Privileged ("root") access to the VM
* Privileged ("root") access to the MySQL server
* Names and email addresses of your designated personnel (e.g. Security Officer and Data Admin) who will manage your Server General deployment
* Ability to export your MySQL server display using "ssh" e.g. ssh -X <IP address of your MySQL server>. If for some reason you are not able to export display of your MySQL server, then you can use our command line interface to configure *Server General KMS for MySQL*.
Our On-boarding Engineer will reach out to your designated contact within 1 business day (excluding US holidays) to assist with setup and configuration.
 
 
### Pricing ###
Our standard pricing for a Server General Agent is $199/month/server. This will allow you to protect your MySQL master encryption key (MMK) as well as your MySQL log files.
 
### Frequently Asked Questions (FAQ) ###
 
#### Will executing this Runner job charge my CenturyLink Cloud account? ####
Yes, executing this Runner job will initiate a recurring monthly subscription. There is no on-boarding charge. You can cancel your service at anytime. You will be charged for the full month in which you cancel service.
 
#### Who should I contact for support? ####
* Please send Server General support requests to: [support@servergeneral.com](mailto:support@servergeneral.com).
* For issues related to CenturyLink Cloud infrastructure (VMs, network, etc.), please open a support ticket by emailing [help@ctl.io](mailto:help@ctl.io) or [through the support website](https://t3n.zendesk.com/tickets/new).
 
#### How difficult is it to deploy? ####
Click the "Run" button to begin the deployment process. Then, populate the Runner job user-input fields with the following:
* Contact information
* E-mail address
* Server Name
* Password/Passphrase for the "sgadmin" user
 
After updating the form fields, click the "Run" button again to initiate the Server General Agent deployment. Once the installation is finished the designated contact will receive an email or phone call from the On-boarding Project Manager (OPM) to schedule time to configure Server General KMS for MySQL. If you like you can configure it yourself as well. The entire process generally takes less than 30 minutes.
 
#### Will authorized MySQL users see the data in clear text format? ####
Yes.
 
#### What is the additional overhead due to encrypting my MySQL data in real-time? ####
According to Oracle, the “performance overhead amounts to a single digit percentage difference”.
 
#### What encryption algorithm is used to encrypt MySQL data? ####
Advanced Encryption Standard (AES) block-based encryption algorithm (Cipher Block Chaining (CBC) block encryption is used secure to MySQL data as well as the MMK.
 
#### Is the data in memory clear-text or encrypted? ####
In-memory data is clear-text.
 
#### Can I use mysqlpump or mysqldump with encrypted tables? ####
Yes. However, your dumped data is not going to be encrypted. You can use Server General encryption to encrypt your backups. Please talk to us we’ll tell you how to go about it.
 
#### Where does *Server General KMS for MySQL* store the MySQL master encryption key? ####
The encrypted value of the MySQL master encryption key (MMK) is stored in a cloud locker managed by Server General security professionals. Alternatively, you can choose to store the master encryption key in a secure, managed key locker appliance deployed on-prem (sold separately).
