<p align="center"><img src="https://github.com/coder-factory-academy/cf-guidline-css/blob/master/CFA.png"></p>

# Setup for Linux
How to setup a linux on your Mac or PC suitable for Ruby on Rails.

Steps:
Skip to step 6 if you are running linux natively.
### Step 1
<img src="http://res.cloudinary.com/coder-factory/image/upload/c_scale,h_128/v1458002275/virtualbox_vxacw1.png">

Visit https://www.virtualbox.org/ and click the download VirtualBox button. Select the version that suits your operating system.

Once downloaded, open the installer and follow the instructions until installed.

### Step 2
Visit https://www.linuxmint.com/download.php and download the MATE 64bit version of linux mint. There are several countries to choose from, any one will do.

### Step 3
Open the VirtualBox application and using the Manager window click the "new" button.
Give it a name, a type with the selection of Linux and version of Ubuntu 64 bit.

If your machine has 4GB of RAM then give the Virtual Machine 1GB (1024MB), if you have 8GB or more then give the VM 2GB (2048MB).

Click continue until you reach "Hard disk".

Choose the "Create a virtual hard disk now" option and click create.

Choose Hard disk file type "VDI" and continue.

Choose "Dynamically allocated" and continue.

Raise the "size limit" from 8GB to 12GB.

This will create your virtual disk that stores the linux operating system to an image file on your computer.

### Step 4
In VirtualBox, while on the Manager window - choose the name of your linux image file and click the button "settings".

Click the "Storage" button icon.

Select the "Empty" on the Controller: IDE and on the right of that window choose the CD icon next to "Optical Drive"

Choose "Virtual Optical Disk Drive", navigate your computer to where you downloaded the linux mint file and select that.

Press ok to close the Settings window.

### Step 5
Select the name of your virtual linux and click the "Start" button icon.

Wait for linux instructions.

A desktop will show with a CD icon of "Install Linux Mint", double-click that to open the installer.

Choose English and click continue.

Ensure you are connected to the internet and have power, click continue.

Have only "Erase disk and install Linux Mint" option selected and click "Install Now".

When asked if you would like to "Write the changes to disks?" click continue.

Choose Sydney as your region and click continue.

Choose English(US) as your keyboard layout and click continue.

Fill out the form details in the "Who are you?" view, choose the "login automatically" option and click continue.

Linux will now install. Once finished click "restart now" and after the restart press "Enter" when prompted.

You will need to unmount the install disk before restart. If necessary shutdown the machine, remove the image, then start it back up.

### Step 6
Open the linux terminal (Mint terminal is bottom left black screen icon).

You may want to enable copy and paste between virtual machine and host:
http://www.howtogeek.com/187535/how-to-copy-and-paste-between-a-virtualbox-host-machine-and-a-guest-machine/

Type these task commands one after another with enter/return.

```
sudo apt-get update
```

```
sudo apt-get install curl git software-properties-common
```

```
sudo apt-get install gawk g++ gcc make libc6-dev libreadline6-dev
```

```
sudo apt-get install zlib1g-dev libssl-dev libyaml-dev libsqlite3-dev sqlite3 autoconf
```

```
sudo apt-get install libgdbm-dev libncurses5-dev automake libtool bison pkg-config libffi-dev
```
