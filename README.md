# Installing Nexus on a VM using Vagrant (MacOS Apple Silicon chip)

Before beginning check [Starterkit](https://github.com/wkwwa/wkwwa/blob/main/starterkit.md)

Step 1. Install rosetta

Open terminal and execute below command
```
/usr/sbin/softwareupdate --install-rosetta --agree-to-license
```
Step 2. Install vagrant with homebrew

Open terminal and execute below command
```
brew install vagrant
```
Step 3. Create an account on Broadcom

Open the link in the browser and click on register.
```
https://support.broadcom.com
```
Step 4. Download & Install VMWare Fusion Tech Preview
  1. Login
  2. Click on top right corner and select VMware Cloud Foundation
  3. Click My Downloads.
  4. Select VMware Fusion
  5. Select VMware Fusion 13 Pro for Personal Use
  6. Select 13.6
  7. Click on the Download Icon
  8. Double click on the downloaded software to start the installation.
  9. Double click on the fusion icon to start the installation and enter the password.

Step 5. Allow vmware Fusion in Accessibility of Security and Privacy Settings.
  1. Open System Settings.
  2. Go to Privacy & Security
  3. Select Accessibility
  4. Toggle on the switch on VMware Fusion

Step 6. Installing vagrant VMware provider.

Open terminal and execute below command.
```
brew install --cask vagrant-vmware-utility
```
Step 7. Install vmware plugin for vagrant

Open terminal and execute below command.
```
vagrant plugin install vagrant-vmware-desktop
```
Step 8. Create folder for ubuntu vm

Open terminal and execute below command.
```
cd
mkdir -p Desktop/vms
cd Desktop/vms
```
Step 9. Bring up vm

Make sure in the terminal, you are in the same folder where Vagrantfile is created.
```
vagrant up
vagrant ssh
sudo -i
ip addr show
exit
exit
vagrant halt
vagrant destroy
```