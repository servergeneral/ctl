![Server General Logo](https://www.servergeneral.com/wp-content/uploads/mediapress/server-general-logo.png)

### Summary
*Server General KMS for MySQL* is a key management service for customers who want to use MySQL TDE to encrypt their data but do not want to build or manage a complicated, expensive and time consuming in-house key management system. With our service in place you will be able to focus on developing your business applications while we manage your MySQL master encryption keys in a secure and compliant manner. Our service enables you to store your encryption keys on-premises or within our cloud locker. Your MySQL server can be hosted on any cloud platform or within your own data center. Customers use our service in order to comply with security requirements of the HIPAA Act and the PCI DSS mandates.

### Description
In 2016 Oracle added Transparent Data Encryption (TDE) feature to the MySQL server. With this new functionality in hand database administrators can now encrypt sensitive information stored in their MySQL database servers to ensure privacy and prevent data breaches. Moreover, the functionality is available for free in the MySQL Community edition. However, both the Community and the Enterprise edition lack proper key management. Oracle recommends the use of Oracle Key Vault (or any other KMIP compliant key locker) for managing MySQL master encryption keys. The cost of such a solution can run into tens of thousands of dollars - a small fortune for many small to medium sized businesses.
Server General KMS for MySQL is a key management service for MySQL customers who want to use the TDE functionality but are not ready to take on the arduous task of building and managing an expensive key management system of their own. The service allows customers to offload their key management responsibilities to us. We have a global key management infrastructure that is managed by our security experts on 24x7x365 basis. We ensure that the encryption keys are stored securely and are available to authorized individuals when needed. Our key management procedures are designed to meet or exceed data compliance requirements of various regulations including that of the HIPAA/HITECH Act.
It usually takes less than 30 minutes to install and configure our service. The service is geared towards small to medium sized businesses.

*Server General KMS for MySQL* is built on top of our secure platform, Server General. The core components of our platform are a data encryption engine, a key management engine, an access control engine, and a reporting engine. Each component performs a critical function in securing the MySQL Master key(MMK).


This diagram illustrates how Server General KMS for MySQL works.

![*Server General KMS for MySQL* Architecture](https://www.servergeneral.com/wp-content/uploads/mediapress/how_does_it_work_kms.png)

### Additional Information
For more details on *Server General KMS for MySQL* architecture, please visit the [Server General Technology page](https://www.servergeneral.com/products/kms/mysql/). 

### Deployment Process
This Runner job performs the following steps:

1. Installs a Server General Agent on your MySQL server deployed within CenturyLink Cloud account and initiates a monthly recurring subscription.
2. Gets hold of basic customer information in order to generate a customer record.
3. Initializes a system user - “sgadmin” in order to manage the Server General TDE installation.
4. Acquires a Server General Agent subscription license and applies it to your server. This step also provisions a cloud key locker account.
5. Notifies the Server General on-boarding team.

### Prerequisite(s)
* Access to the CenturyLink Cloud platform as an authorized user.
* Access to Ubuntu 14.04 or Ubuntu 16.04 or Debian-7 or Debian-8 or RHEL-6.x or CentOS-6.x virtual machine with a MySQL server 5.7.12 (or a higher release).
* Contact information for the designated administrative contact.

### Postrequisite(s)
* Privileged ("root") access to the VM
* Privileged ("root") access to the MySQL server
* Names and email addresses of your designated personnel who will manage your Server General deployment
* Ability to export your MySQL server display using "ssh" e.g. ssh -X <IP address of your MySQL server>. If for some reason you are not able to export display of your MySQL server, then you can use our commandline interface to configure *Server General KMS for MySQL*.

### Pricing
Our standard pricing for a Server General Agent is $199/month/server. This will allow you to protect your MySQL master encryption key as well as your MySQL log files.

### Frequently Asked Questions (FAQ)

#### Will executing this Runner job charge my CenturyLink Cloud account?
Yes, executing this Runner job will initiate a recurring monthly subscription. There is no on-boarding charge. You can cancel your service at anytime. You will be charged for the month in which you cancel your service.

#### Who should I contact for support?
* Please send support requests to: [support@servergeneral.com](mailto:support@servergeneral.com).
* For issues related to CenturyLink Cloud infrastructure (VMs, network, etc.), please open a support ticket by emailing [help@ctl.io](mailto:help@ctl.io) or [through the support website](https://t3n.zendesk.com/tickets/new).

#### How difficult is it to deploy?
Click the "Run" button to begin the deployment process. Then, populate the Runner job user-input fields with the following:
* Contact information
* E-mail address
* Server Name
* Password/Passphrase for the "sgadmin" user

After updating the form fields, click the "Run" button again to initiate the Server General Agent deployment. Once the installation is finished the designated contact will receive an email or phone call from the On-boarding Project Manager (OPM) to schedule time to configure Server General KMS for MySQL. If you like you can configure it yourself as well. The entire process generally takes less than 30 minutes.

#### Can authorized MySQL users see the data in clear text format?
Yes.

#### What is the overhead associated with type of an approach to encryption?
According to Oracle the “performance overhead amounts to a single digit percentage difference”.

#### What encryption algorithm is used to encrypt MySQL data?
Advanced Encryption Standard (AES) block-based encryption algorithm (Cipher Block Chaining -CBC- block encryption is used to MySQL data).

#### Does database memory contain clear-text or encrypted data?
In-memory data is decrypted.

#### Can I use mysqlpump or mysqldump with encrypted tables?
Yes. However, your dumped data is not going to be encrypted. You can use Server General encryption to encrypt your backups. It will cost you $99.99/month extra.

#### Where does Server General store the MySQL master encryption key?
The encrypted value of the master encryption key is stored in a cloud locker managed by Server General security professionals. You have the option of storing the master key in a virtual appliance deployed within your own network.
