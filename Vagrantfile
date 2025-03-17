Vagrant.configure("2") do |config|
  config.vm.box = "roboxes/ubuntu2204"
  config.vm.provider "virtualbox"
  config.vm.hostname = "LuizPhilipe"
  config.vm.network "private_network", ip: "192.168.57.10"
  config.vm.network "forwarded_port", guest: 80, host: 8080


  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook_ansible.yml"
  end
end
