# -*- mode: ruby -*-
# vi: set ft=ruby tabstop=2 :
box_url = "http://opscode-vm-bento.s3.amazonaws.com/vagrant/virtualbox/opscode_centos-6.6_chef-provisionerless.box"

Vagrant.configure("2") do |config|
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.hostname  = "devops-bootcamp.osuosl.org"
  config.vm.box_url   = "#{box_url}"
  config.vm.network "forwarded_port", guest: 80, host: 8080, auto_correct: true
  config.vm.network "forwarded_port", guest: 5000, host: 5050, auto_correct: true
  config.vm.provider :virtualbox do |vb|
    # uncomment to enable GUI console
    #vb.gui = "true"
    # uncomment to disable hardware virt
    #vb.customize ["modifyvm", :id, "--hwvirtex", "off"]
    end
end
