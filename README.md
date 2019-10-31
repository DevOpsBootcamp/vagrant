Devops Bootcamp Vagrant Environments
====================================

A set of vagrant environments used by the [Devops Bootcamp](http://devopsbootcamp.osuosl.org).

Installing Dependencies
-----------------------

Do not use the version of Vagrant that comes from your system's package manager unless you know it's up to date (if
you're running an Ubuntu derivative, it won't be). Instead, download the appropriate package from [the Vagrant
site](http://www.vagrantup.com/downloads.html).

Additionally, get a recent version of VirtualBox from [their download page](https://www.virtualbox.org/wiki/Downloads).
If you're running Linux, you'll also need to install the ``virtualbox-dkms`` package from your package manager for the
necessary kernel modules. You may also install VMWare Workstation if you have access to it as an alternative.

Starting your VM
----------------

Now you can use the ``Vagrantfile`` in this repo to create your vagrant VM:

``` console
$ git clone git@github.com:DevOpsBootcamp/vagrant.git
$ cd vagrant
# Start a CentOS VM
$ vagrant up    # Download image and start VM
$ vagrant ssh   # to get into your VM

# Start a Ubuntu VM
$ cd ubuntu
$ vagrant up    # Download image and start VM
$ vagrant ssh   # to get into your VM

# Start a Debian VM
$ cd debian
$ vagrant up    # Download image and start VM
$ vagrant ssh   # to get into your VM

```

Troubleshooting
---------------

If you get any errors, Google them and use the VirtualBox and Vagrant documentation to resolve them.

If it hangs on the ``vagrant ssh`` part for several minutes, try accessing the VM through the VirtualBox interface to
see what error it's displaying on its console, then Google that error and fix your VirtualBox installation.
