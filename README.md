Devops Bootcamp Vagrant Environments
====================================

A set of vagrant environments used by the [Devops Bootcamp][1].

[1]: http://devopsbootcamp.osuosl.org

Installing Dependencies
-----------------------

Do not use the version of Vagrant that comes from your system's package manager
unless you know it's up to date (if you're running an Ubuntu derivative, it
won't be). Instead, download the appropriate package from [the Vagrant site][2].

[2]: http://www.vagrantup.com/downloads.html

Additionally, get a recent version of VirtualBox from [their download page][3]. 
If you're running Linux, you'll also need to install the virtualbox-dkms
package from your package manager for the necessary kernel modules. 

[3]: https://www.virtualbox.org/wiki/Downloads

Now you can use the Vagrantfile in this repo to create your vagrant VM: 

```
$ git clone git@github.com:DevOpsBootcamp/devopsbootcamp-vagrant.git
$ cd devopsbootcamp-vagrant
$ vagrant up
$ vagrant ssh           # to get into your VM
```

32 bit Virtual Machine
----------------------
If you are having trouble using the default Vagrantfile because it uses a 64 bit VM,
there is a 32 bit VM available. Simply replace the `Vagrantfile` 
with `Vagrantfile-32bit` by running:
```sh
$ mv Vagrantfile-32bit Vagrantfile
```
Then, continue as normal.


Troubleshooting
---------------

If you get any errors, Google them and use the VirtualBox and Vagrant
documentation to resolve them. 

If it hangs on the `vagrant ssh` part for several minutes, try accessing the VM
through the VirtualBox interface to see what error it's displaying on its
console, then Google that error and fix your VirtualBox installation.
