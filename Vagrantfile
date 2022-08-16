Vagrant.configure(2) do |config|
    config.vm.box = "generic/ubuntu1804"
    # https://app.vagrantup.com/generic/boxes/ubuntu1804
   
    config.vm.provider "virtualbox" do |v|
      v.name = "htpc.dev"
      v.memory = 2048
      v.cpus = 2
    end

    config.vm.provider "hyperv" do |h|
        h.enable_virtualization_extensions = true
        h.vmname = "htpc.dev"
        h.memory = 2048
        h.cpus = 2
    end
   
    config.vm.provision "ansible_local" do |ansible|
      ansible.verbose = "vvv"
 #     ansible.extra_vars = { "ansible_python_interpreter" => "/usr/bin/python2" }
      ansible.playbook = "main.yml"
      ansible.groups = {
          "localhost" => ["localhost"]
      }
    end
 end