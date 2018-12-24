# Task OVPNC

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.provision :shell, path: "bootstrap.sh"
  config.ssh.insert_key = false


  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "main.yml"
  end
end
