![Server General logo](https://www.servergeneral.com/wp-content/uploads/mediapress/server-general-logo.png)

### Summary
*Server General TDE* is a data security service that makes it easy to protect sensitive information stored in a database server or a file server deployed anywhere - public, private or a hybrid cloud. 
 
Developed by encryption experts, *Server General TDE* provides data encryption and key management, enabling you to take a concrete step towards achieving regulatory compliance with HIPAA/HITECH, PCI DSS mandates, GDPR, FISMA, GLBA, SOX and FERPA. *Server General TDE* has been certified to encrypt data stored in a MySQL, PostgreSQL, MongoDB, CouchDB or a File server. 
 
Our simple _key management system_ enables key generation, storage, rotation and revocation all in just a few steps. Typically, the time to configure and encrypt your database or file server is less than 30 minutes. This solution is ideal for small to medium-sized businesses who want to secure their data, fulfill compliance requirements, and do it all at a fraction of the cost charged by traditional security providers.


### Description
Managing and securing customer and employee data is a growing concern of all Information Technology (IT) departments, especially when operating in the cloud. Organizations try hard to comply with regulations and industry mandates, but the effort required often exceeds the capability of small IT groups. *Server General TDE* enables organizations to focus on their business while making it easy for them to encrypt their data and manage their encryption keys -- all in a compliant manner. 
 
*Server General TDE* uses industry standard AES encryption to encrypt data at the file system layer. Our solution transparently encrypts sensitives file with a unique random key. All privileged operations conducted by administrators are logged within and outside of the administrative domains of our customers in order to provide non-repudiation. Management responsibilities are segregated based on roles (Security Officer, Data Admin) to effectively safeguard data. Customers can store encryption keys on-premises in a secure, managed key locker appliance, or use our secure cloud key locker infrastructure (both services sold separately).


![*Server General TDE*](https://www.servergeneral.com/wp-content/uploads/SERVER-GENERAL-TDE-DIAGRAM-2017.jpg)

This diagram illustrates how Server General TDE works.

![*Server General TDE* Architecture](https://www.servergeneral.com/wp-content/uploads/how_does_it_works_TDE_web_2017.jpg)

### Additional Information
For more details on *Server General TDE* architecture, please visit the [Server General TDE product offering page](https://www.servergeneral.com/products/tde/) on our website. 

### Deployment Process
This Runner job performs the following steps:

1. Installs a Server General Agent on your CenturyLink Cloud server and initiates a monthly recurring subscription.
2. Initializes a system user - “sgadmin” in order to manage the Server General TDE installation.
3. Acquires a Server General Agent subscription license and applies it to your server. This step also provisions a cloud key locker account.
4. Notifies the Server General on-boarding team who will contact you within 1 business day.

### Prerequisite(s)
* Access to the CenturyLink Cloud as an authorized user.
* Confirm the target server OS is one of the following: Ubuntu 14.04, Ubuntu 16.04, Debian-7, Debian-8, RHEL-6.x, CentOS-6.x.
* Contact information for the designated administrative contact.
 
### Post-requisite(s)
* Privileged ("root") access to your virtual server.
* Names and email addresses of your designated personnel (e.g. Security Officer and Data Admin) who will manage your Server General deployment.
* Our On-boarding Engineer will reach out to your designated contact within 1 business day (excluding US holidays) to assist with setup and configuration.
 
### Pricing
Our standard pricing for a Server General Agent is $199/month/server. 










