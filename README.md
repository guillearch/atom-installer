# AtoM 2.4 Ubuntu 16.04 LTS Installer

This simple script will help you to install the most stable release of AtoM in Ubuntu 16.04 LTS along with all the required third party components. At the end you should get AtoM 2.4 running in a Nginx server. Some manual tasks will be needed during the process.

This installer was created by [Guillermo Castellano](https://guillearch.github.io/), from [Nosturi](https://nosturi.es/).

The code is licensed under the [GNU General Public License v3.0](https://github.com/guillearch/atom-installer/blob/master/LICENSE). Feel free to adapt the script for your needs!

##Requirements

This script is intended for a fresh Ubuntu 16.04 LTS install and may not work properly in other environments.

Note that you will have to run a web installer to complete the install. If you are working remotely, you will need to set up X11 forwarding first.

Please make sure you have sudo privileges before continuing.

##Downloading the installer

Let's clone the repository with the following command:

```
git clone https://github.com/guillearch/atom-installer.git
```

Alternatively, you can download it as a ZIP:

```
wget https://github.com/guillearch/atom-installer/archive/master.zip
```

Then unzip the file:

```
unzip master.zip
```

##Running the script

Run the script by entering the following command:

```
sudo sh atominstaller.sh
```

Insert your user password.

Set the password for the Percona Server root user.

Answer "no" when the installer asks you if you want to enable internal debugging in APCu.

You will be prompted to type again the password you chose earlier.

##Running the web installer

The script will ask you to run the web installer in order to complete the install. To do so, open your browser and type "localhost" in the address bar.

To configure the database, enter the following information:

* Database name: `atom`
* Database username: `atom`
* Database password: `12345`
* Database host: `localhost`
* Database port: `3306`

To configure the search engine, enter the following information:

* Search host: `localhost`
* Search port: `9200`
* Search index: `atom`

Finally, the installer will ask you to enter a title, description and base URL for your site and set up the administrator account.

##Additional information

This installer is based on the [AtoM 2.4 documentation](https://www.accesstomemory.org/es/docs/2.4/#) provided by Artefactual Systems.

If you need any further assistance, don't hesitate to [contact me](mailto:gcastellano@nosturi.es).

Keep calm and use ISAD (G)!
