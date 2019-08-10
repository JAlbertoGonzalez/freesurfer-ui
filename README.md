# Freesurfer UI

Windows Subsystem for Linux
-----------

Freesurfer v6.0.0 is only available for Linux and MacOS.

In order to install Freesurfer in a Windows subsystem, you could create a new virtual machine using Virtual Box, or you can install WSL (Windows Subsystem for Linux) in your Windows 10 machine.

To enable WSL:

* Open **start**
* Search for **Turn Windows features on or off**
* Check the **Windows Subsystem for Linux** option
* Click the **OK** button
* Click **Restart** button.

Once WSL is enabled, install the latest Ubuntu.

* Open **start**
* Search for **Windows Store**
* Inside Windows Store, search **Ubuntu** (by Canonical Group Limited)
* Click **Install** button.

After install, you can open a Ubuntu shell window clicking on Start Menu, and searching Ubuntu app.

Optional: The first time you open the linux shell, you can update all your Linux dependencies by running this command:

```
sudo apt update && sudo apt upgrade
```

Installation of Freesurfer v6.0.0
-

Freesurfer tar.gz file must be uncompressed and placed in a system directory (/usr/local).

* Install wget to be able to download network files in your machine using the command line tool
```
sudo apt install wget
```

* Download the installation file. This may take 2h (4.6GB)
```
wget https://surfer.nmr.mgh.harvard.edu/pub/dist/freesurfer/6.0.0/freesurfer-Linux-centos6_x86_64-stable-pub-v6.0.0.tar.gz
```

* Unzip and place the freesurfer software in your system.
```
tar -C /usr/local -xzvf freesurfer-Linux-centos6_x86_64-stable-pub-v6.0.0.tar.gz
```



License
-

The core application of Freesurfer requires a License key. This licence is free. You only are required to register in this url, and a valid key file will be sent to your inbox.

https://surfer.nmr.mgh.harvard.edu/registration.html

Once you have received your license key, copy the three lines and paste it with your favourite text editor in /usr/local/freesurfer/.license

```
nano /usr/local/freesurfer/.license
```

(You can save and exit with nano editor pressing Control+O, type yes, and then Control+X)

