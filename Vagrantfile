Vagrant.configure("2") do |config|

    config.vm.synced_folder '.', '/vagrant', disabled: true
      
    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
    end

    config.vm.box_url = "maier/alpine-3.1.3-x86_64"

    config.vm.define "docker1" do |docker1|
        docker1.vm.box = "maier/alpine-3.1.3-x86_64"
    end

    config.vm.define "docker2" do |docker2|
        docker2.vm.box = "maier/alpine-3.1.3-x86_64"
    end

    config.vm.define "docker3" do |docker3|
        docker3.vm.box = "maier/alpine-3.1.3-x86_64"
    end

    config.vm.define "docker4" do |docker4|
        docker4.vm.box = "maier/alpine-3.1.3-x86_64"
    end

end
