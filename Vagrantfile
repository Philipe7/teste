Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/jammy64"
    config.vm.hostname = "p01_LuizPhilipe"
    config.vm.network "private_network", type: "dhcp"
  
    config.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook_ansible.yml"
    end
  end
  