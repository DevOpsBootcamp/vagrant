# -*- mode: ruby -*-
# vi: set ft=ruby tabstop=2 :
box_ver = "20131003"
box_url = "http://ftp.osuosl.org/pub/osl/vagrant/centos-6-#{box_ver}.box"

Vagrant.configure("2") do |config|
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box       = "centos-6-#{box_ver}"
  config.vm.hostname  = "devops-bootcamp.osuosl.org"
  config.vm.box_url   = "#{box_url}"
  config.vm.network "forwarded_port", guest: 80, host: 8080, auto_correct: true

  # Boot with a GUI so you can see the screen. (Default is headless)
  # config.vm.boot_mode = :gui
end
