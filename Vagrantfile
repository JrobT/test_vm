Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-16.04"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "8192"
    vb.name = "test machine"
  end

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "ansible/vagrant.yml"
    ansible.become = true
  end
end