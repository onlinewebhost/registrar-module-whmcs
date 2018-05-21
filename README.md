### connectreseller.com WHMCS Registrar Plugin

***

##### [ReleaseNotes](https://github.com/namecheap/domains-whmcs/wiki/Changelog)

connectreseller.com WHMCS Registrar plug-in is an open-source plug-in that is distributed free of charge. It focuses on integrating ConnectReseller as a domain registrar at WHMCS.

After the integration you can setup ConnectReseller as the default registrar for your customers and decide which services and TLDs to offer to your customers from within the WHMCS admin area.

##### Pre-requisites

- Access to WHMCS admin area.
- An understanding of ConnectReseller environments.
- ConnectReseller account .


##### Download and Installation

- Download the latest plugin (connectreseller-whmcs.x.x.zip) archive and extract it.
- Create a folder called connectreseller under Modules/Registrar in your WHMCS root directory and paste the downloaded connectreseller.php and logo.gif file inside the folder (the connectreseller.php and logo.gif file are located inside the downloaded archive). The plug-in installation is complete.

##### Configuration

To configure WHMCS for use with ConnectReseller, perform the following steps:

1. Login to your **WHMCS admin** panel.
2. Click on **Setup** menu, select **Products/Services** and click on **Domain Registrars**.
3. Click on Activate next to ConnectReseller in the list:
 ![Activate Plugin](https://global.connectreseller.com//images/activate.jpg "Activate Plugin")

4. Enter your API credentials. Enter the API Key and Brand Id 
(To know your API key and brand ID, Once you have logged in, Go to Profile > Brand URL > API )
	![Activate Plugin](https://global.connectreseller.com//images/config.png "Configure Plugin")
5. Click Save Changes.


That’s it. The ConnectReseller plug-in is now ready for use and will function just like any other built-in WHMCS registrar module. You can now make ConnectReseller as the automatic registrar, configure TLDs and services for all your customers. To perform these actions, click on the Setup menu, select Products/Services and click on Domain Pricing in your WHMCS admin panel:

Note: 
1. You need to whitelist your WHMCS IP Address into you ConnectReseller panel.
2. This step is for your server, if it does not have a latest version of CA certificate of COMODO installed. If you were unable to Register the domain and encounter with the error "cURL error (60): Peer certificate cannot be authenticated with given CA certificates", then you have to proceed with this last step.
3. You first have to copy the file "combined.pem" (this file includes latest Comodo CA certificate, you can open it as txt file to see) in the /tmp folder under your server directory. Once you have copied the file, then you must run the command: cat /tmp/combined.pem >> /etc/pki/tls/certs/ca-bundle.crt as this will update the latest CA certificate in your server. -The CA certificate is present in the zip file named as combined.pem, you can open it as a text file. cat /tmp/combined.pem >> /etc/pki/tls/certs/ca-bundle.crt 
4. Kindly do the needful with the help of your system administrator and also update the WHMCS to the latest version if it hasn't been updated yet.



##### Support

Please [submit a ticket](http://support.connectreseller.com) to report bugs, provide feedback or receive assistance.