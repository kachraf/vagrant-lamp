
Vagrant.configure(2) do |config|

  config.vm.box = "hashicorp/precise64"
  # Mentioning the SSH Username/Password:
  config.ssh.username = "vagrant"
  config.ssh.password = "vagrant"
  # Begin Configuring
  config.vm.define "lamp" do|lamp|
  lamp.vm.hostname = "lamp" # Setting up hostname
  lamp.vm.network "private_network", ip: "192.168.205.10" # Setting up machine's IP Address
  lamp.vm.provision :shell, path: "script.sh" # Provisioning with script.sh
  end
# End Configuring
end