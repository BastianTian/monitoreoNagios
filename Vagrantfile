Vagrant.configure("2") do |config|

  if Vagrant.has_plugin? "vagrant-vbguest"
     config.vbguest.no_install = true
     config.vbguest.auto_update = false
     config.vbguest.no_remote = true
  end
  config.vm.define :nagios do |nagios|
    nagios.vm.provision "shell", path: "nagios.sh.txt"
    nagios.vm.box = "bento/centos-7.9"
    nagios.vm.network :private_network, ip: "192.168.100.2"
    nagios.vm.hostname = "nagios"
    nagios.vm.provider "virtualbox" do |v|
      v.cpus = 2 
    end
  end
  config.vm.define :cliente2 do |cliente2|
    cliente2.vm.provision "shell", path: "cliente2.sh.txt"
    cliente2.vm.box = "bento/centos-7.9"
    cliente2.vm.network :private_network, ip: "192.168.100.3"
    cliente2.vm.hostname = "cliente2"
    cliente2.vm.provider "virtualbox" do |v|
      v.cpus = 2 
    end
  end
  config.vm.define :cliente1 do |cliente1|
    cliente1.vm.provision "shell", path: "cliente1.sh.txt"
    cliente1.vm.box = "bento/centos-7.9"
    cliente1.vm.network :private_network, ip: "192.168.100.4"
    cliente1.vm.hostname = "cliente1"
    cliente1.vm.provider "virtualbox" do |v|
      v.cpus = 2 
    end
  end
end