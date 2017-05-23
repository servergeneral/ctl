![Server General logo](https://www.servergeneral.com/wp-content/uploads/mediapress/server-general-logo.png)

### Summary
*Server General TDE* is a data encryption service that makes it easy to set-up, maintain, manage and administer data-at-rest encryption of your sensitive information stored in a database server or a file server deployed anywhere - public, private or a hybrid cloud. The service will allow you to offload your data encryption and key management responsibilities to proven experts while taking a concrete step towards achieving regulatory compliance with HIPAA/HITECH, PCI DSS mandates, GDPR, FISMA, GLBA, SOX and FERPA. *Server General TDE* has been certified to encrypt data stored in a MySQL, PostgreSQL, MongoDB, CouchDB or a file server. The service includes a full featured key management system that provides key generation, storage, rotation and revocation. It usually takes less than 30 minutes to install and configure our service. The service is geared towards small to medium sized businesses who want to cut their data security and compliance costs.

### Description
Managing and securing customer and employee data is a growing concern of all Information Technology departments, especially when operating in the cloud. Organizations try hard to comply with regulations and industry mandates, but the effort necessary often exceeds the capability of small IT groups. *Server General TDE* being a service allows such organizations to focus on their business while helping them to encrypt their data and manage their encryption keys in a compliant manner. We use the AES encryption algorithm to encrypt data at the file system layer. Our service is designed to transparently encrypt each and every sensitive file with a unique and completely random key. All privileged operations conducted by the Server General administrators are logged within and outside of the administrative domains of our customers in order to provide non-repudiation. The service segregates management responsibilities based on roles in order to safeguard data. We provide an option to store the encryption keys on-premises in a secure appliance or within our secure cloud key locker infrastructure. It generally takes less than 30 minutes to install and configure our service.

![*Server General TDE*](https://www.servergeneral.com/wp-content/uploads/TDE-diagram.jpg)

<<Server General TDE graphic goes here>>

This diagram illustrates how Server General TDE works.

![*Server General TDE - How does it work*](https://www.servergeneral.com/wp-content/uploads/mediapress/how_does_it_work_kms.png)

### Additional Information
For more details on *Server General TDE* architecture, please visit the Server General TDE product offering page on our website.

### Deployment Process
This Runner job performs the following steps:

1. Installs a Server General Agent on your server deployed within CenturyLink Cloud account and initiates a monthly recurring subscription.
2. Gets hold of basic customer information in order to generate a customer record.
3. Initializes a system user - “sgadmin” in order to manage the Server General TDE installation.
4. Acquires a Server General Agent subscription license and applies it to your server. This step also provisions a cloud key locker account.
5. Notifies the Server General on-boarding team.

### Prerequisite(s)
* Access to the CenturyLink Cloud platform as an authorized user.
* Access to Ubuntu 14.04 or Ubuntu 16.04 or Debian-7 or Debian-8 or RHEL-6.x or CentOS-6.x virtual server.
* Contact information for the designated administrative contact.

### Postrequisite(s)
* Privileged ("root") access to your virtual server
* Names and email addresses of your designated personnel who will manage your Server General deployment

### Pricing
Our standard pricing for a Server General Agent is $199/month/server. Here is how our pricing differs from our competitor:

Number of servers = 1
Vormetric
Server General
TCO - Year - 1
$14,372
$2,400
TCO - Year - 2
$12,372
$2,400
TCO - Year - 3
$12,372
$2,400
Total TCO for 3 years
$39,116
$7,200