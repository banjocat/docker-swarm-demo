Vagrant.configure("2") do |config|

    config.vm.synced_folder '.', '/vagrant', disabled: true
    config.vm.box = "ubuntu/trusty64"
    config.vm.box_url = "ubuntu/trusty64"

      
    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
    end

    config.vm.define "manager" do |manager|
        manager.vm.network "private_network", ip: "10.0.1.2"
    end

    config.vm.define "node0" do |node0|
        node0.vm.network "private_network", ip: "10.0.1.3"
    end

    config.vm.define "node1" do |node1|
        node1.vm.network "private_network", ip: "10.0.1.4"
    end

    config.vm.define "node2" do |node2|
        node2.vm.network "private_network", ip: "10.0.1.5"
    end


end
