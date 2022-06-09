# vagrantfile
Vmware:

Open CMD:
```
vagrant plugin install vagrant-vmware-desktop

https://www.vagrantup.com/docs/providers/vmware/installation
https://www.vagrantup.com/vmware/downloads
```


## create a file name: Vagrantfile
```
Vagrant.configure("2") do |config|
  config.vm.define "master" do |subconfig|
    subconfig.vm.box = "bento/ubuntu-20.04"
  end

  config.vm.define "node1" do |subconfig|
    subconfig.vm.box = "bento/ubuntu-20.04"
  end
end
```
```
vagrant up --provider vmware_desktop
```
