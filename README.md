# vagrantfile

Vmware:

Open CMD:

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

