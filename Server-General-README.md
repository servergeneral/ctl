![Server General Logo](http://kms.servergeneral.com/mediapress/server-general-logo.png)

### Summary
*Server General KMS for MySQL* is a key management service for customers who want to use MySQL TDE to encrypt their data but do not want to build or manage a complicated, expensive and time consuming in-house key management system. With our service in place you will be able to focus on developing your business applications while we manage your MySQL master encryption keys in a secure and compliant manner. Our service enables you to store your encryption keys on-premises or within our cloud locker. Your MySQL server can be hosted on any cloud platform or within your own data center. Customers use our service in order to comply with the HIPAA Act and PCI DSS mandates with ease.

### Description
*Server General KMS for MySQL* is built on top of our secure platform, Server General. The core components of our platform are a data encryption engine, a key management engine, an access control engine, and a reporting engine. Each component performs a critical function in securing the MySQL Master key(MMK).

* **Fully Managed Service** <br>
Organizations try hard to comply with regulations and industry mandates, but the effort necessary often exceeds the capability of small IT groups. *Server General KMS for MySQL* being a service allows such organizations to focus on their business while we help them manage their MySQL encryption keys in a compliant manner. It generally takes less than 30 minutes to install and configure our service. Our service allows you to control your own encryption keys while we ensure their availability and security.
* **Works With All Cloud Platforms** <br>
*Server General KMS for MySQL* allows you to centralize and manage your encryption keys for your MySQL servers spread across distributed cloud platforms - Amazon, CenturyLink, Google, Rackspace or within your own data center.
* **Store Keys On-Premises Locker or a Cloud Locker** <br>
You have the option of storing your MySQL encryption keys in a secure appliance deployed on-premises or within our cloud lockers. We encrypt your MySQL master encryption key with a key that is only known to you. This way we never have access to the actual encryption key.
* **Low-cost** <br>
Unlike other vendors whose key management solutions can easily cost you thousands of dollars we see ourselves as a no-frills service provider. You can start for as little as $199/month/server.
* **Security** <br>
Our on-premises key locker is a battle hardened virtual appliance while our cloud key management infrastructure is managed by our security experts on 24x7x365 basis. All privileged operations are logged at four different locations in order to provide non-repudiation. The MySQL master encryption key is not stored on your server but in a key locker. It’s important to point out that we only store the encrypted value of your encryption key in our key lockers. This way our staff is unable to access the real encryption key. At the same time if your server were to be compromised the key remains out of reach of an attacker as it is not stored on the server. When the key is needed to restart the MySQL service, our agent fetches the encrypted value from our key locker and only the data owner is able to reconstitute the actual encryption key using a secret passphrase. Furthermore, we use advanced access control mechanisms to deny the “root” user access to the key when it is being used on the server for a very brief period.
* **Compliance** <br>
*Server General KMS for MySQL* stores your MySQL encryption key away from your encrypted data sets which is generally one of the main requirements of any data security regulation. You are further able to limit the scope of your compliance by deploying the key locker within your own network. Our key management system provides key generation, storage, rotation and revocation capabilities. We generate immutable logs of all privileged operations conducted by the Server General administrators by storing them at four different locations.


This diagram illustrates how Server General KMS for MySQL for MySQL works.

![*Server General KMS for MySQL* Architecture](https://www.servergeneral.com/mediapress/kms-mysql/how_does_it_work_kms.png/)

### Additional Information
For more details on *Server General KMS for MySQL* architecture, please visit the [Server General Technology page](https://www.servergeneral.com/products/kms-mysql/technology/).

### Deployment Process
This Runner job performs the following steps:

1. Installs a Server General Agent on your MySQL server deployed within CenturyLink Cloud account and initiates a monthly recurring subscription.
2. Gets hold of basic customer information in order to generate a customer record.
3. Will initialize a special system user called "sgadmin". 
4. Provisions a Server General Agent license.
5. Notifies the Server General on-boarding team.

### Prerequisite(s)
* Access to the CenturyLink Cloud platform as an authorized user.
* Access to Ubuntu 14.04 or Ubuntu 16.04 or Debian-7 or Debian-8 or RHEL-6.x or CentOS-6.x virtual machine with a MySQL server 5.7.12 (or a higher release).
* Contact information for the designated administrative contact.

### Postrequisite(s)
* Privileged ("root") access to the VM
* Privileged ("root") access to the MySQL server
* Names and email addresses of your designated personnel who will manage your Server General deployment
* Ability to export your MySQL server display using "ssh" e.g. ssh -X <IP address of your MySQL server>

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
