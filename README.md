# Setting up the VM
This repo will help you setup the VM

## Ubuntu

You can download an Ubuntu image here. Make sure to save it to a memorable location on your PC! For this tutorial, we will use the <a href="https://releases.ubuntu.com/focal/"> Ubuntu 20.04 release </a>. _Do not install it_.

## Virtual Box 7

In this tutorial, I’ll walk you through one of the easiest ways to try out Ubuntu Desktop on a virtual machine. VirtualBox is a general purpose virtualiser that is available across Linux, Mac OS and Windows. It’s a great way to experience Ubuntu regardless of your current operating system. Please download the virtual box for the operating system you are using <a href="https://www.virtualbox.org/wiki/Downloads"> from here </a>.

Once you have completed the installation, go ahead and run VirtualBox.

![Virtual Box 7 start page](/image1.png)

## Create a new virtual machine

Click New to create a new virtual machine. Fill in the appropriate details:

  -  Name: If you include the word Ubuntu in your name the Type and Version will auto-update.
  -  Machine Folder: This is where your virtual machines will be stored so you can resume working on them whenever you like.
  - ISO Image: Here you need to add a link to the ISO you downloaded from the Ubuntu website.

We want to install Ubuntu unattendedly so we can leave the checkbox to skip unchecked.

![Virtual Box 7 image 2](/image2.png)

## Create a user profile

To enable the automatic install we need to prepopulate our username and password here in addition to our machine name so that it can be configured automatically during first boot.

The default credentials are:

  - Username: vboxuser
  - Password: changeme

Ensure your Hostname has no spaces to proceed!

![Virtual Box 7 image 3](/image3.png)

It is also recommended to check the Guest Additions box to install the default Guest Additions ISO that is downloaded as part of VirtualBox. Guest additions enables a number of quality of life features such as changing resolution and dynamic screen resizing so it is highly recommended!

## Define the Virtual Machine’s resources

In the next section we can specifiy how much of our host machine’s memory and processors the virtual machine can use. For good performance it’s recommended to provide your VM with around 8GB of RAM (althought 4GB will still be usable) and 4 CPUs. Try to remain in the green areas of each slider to prevent issues with your machine running both the VM and the host OS.

![Virtual Box 7 image 4](/image4.png)

Then we need to specify the size of the hard disc for the virtual machine. For Ubuntu we recommend around 25 GB as a minimum. By default the hard disk will scale dynamically as more memory is required up to the defined limit. If you want to pre-allocate the full amount, check the ‘Pre-allocate Full Size’ check box. This will improve performance but may take up unnecessary space.

![Virtual Box 7 image 5](/image5.png)

Click Next to continue and view a summary of your machine setting.

![Virtual Box 7 image 6](/image6.png)

## Install your image

Click Start to launch the virtual machine.

You will see a message saying ‘Powering VM up …’ and your desktop window will appear.

On first boot the unattended installation will kick in so do not interact with the prompt to ‘Try and Install Ubuntu’ and let it progress automatically to the splash screen and into the installer.

You will notice at this stage that the resolution of the window is fixed at 800x600. This is because the Guest Additions features are not installed until after the Ubuntu installation has completed.

Once the installation completes, the machine will automatically reboot to complete the installation.

Finally you will be greated with the Ubuntu log-in screen where you can enter your username and password defined during the initial setup (don’t forget that the default password is ‘changeme’ if you left everything as the default).
