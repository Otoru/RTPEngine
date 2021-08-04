Vagrant.configure("2") do |config|
  config.vm.box = "debian/buster64"

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update -y 
    apt-get install -y ansible
    mkdir -p /vagrant/tests/roles
    ln -s /vagrant/ /vagrant/tests/roles/rtpengine
  SHELL
end
