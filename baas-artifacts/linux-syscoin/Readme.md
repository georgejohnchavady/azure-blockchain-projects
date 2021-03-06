# Syscoin Blockchain Node on Ubuntu VM

This template delivers the Syscoin network to your VM in about 15 minutes (PPA install).  Everything you need to get started using the Syscoin blockchain from the command line is included. 
You may select to build from source or install from the community provided Personal Package Archive (PPA).  Once installed, 'syscoind' will begin syncing the public blockchain. 
You may then connect via SSH to the VM and launch 'syscoind' to interface with the blockchain.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fsyscoin-on-ubuntu%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fsyscoin-on-ubuntu%2Fazuredeploy.json" target="_blank"><img src="http://armviz.io/visualizebutton.png"/></a>

# What is Syscoin?

What is Syscoin?
----------------

Syscoin is a merge-minable scrypt coin which provides an array of useful services
which leverage the bitcoin protocol and blockchain technology.

 - 1 minute block targets
 - Merge mining with Bitcoin network (SHA)


Services include:

- Alias reservation, ownership & exchange. Public/Private profile information.
- Data storage
- Digital document storage, ownership & exchange
- Distributed marketplate & exchange
- Digital Certificates
- Integrated Escrow with Arbitration
- Distributed encrypted communication

For more information, as well as an immediately useable, binary version of
the Syscoin client sofware, see http://www.syscoin.org.


# Template Parameters

When you click the Deploy to Azure icon above, you need to specify the following template parameters:

* `adminUsername`: This is the account for connecting to your Syscoin host.
* `adminPassword`: This is your password for the host.  Azure requires passwords to have One upper case, one lower case, a special character, and a number.
* `dnsLabelPrefix`: This is used as both the VM name and DNS name of your public IP address.  Please ensure an unique name.
* `installMethod`: This tells Azure how to install the software.  The default is using the community provided PPA.  You may choose to install from source, but be advised this method takes substantially longer to complete.
* `vmSize`: This is the size of the VM to use.  Recommendations: Use the A series for PPA installs, and D series for installations from source.

# Getting Started Tutorial

* Click the `Deploy to Azure` icon above
* Complete the template parameters, choose your resource group, accept the terms and click Create
* Wait about 15 minutes for the VM to spin up and install the software
* Connect to the VM via SSH using the DNS name assigned to your Public IP
* If you wish to relaunch syscoind `sudo syscoind`
* syscoind will run automatically on restart

# Licensing

Syscoin is released under the terms of the MIT license. See `COPYING` for moreinformation or see http://opensource.org/licenses/MIT.