
$useraddscript = <<SCRIPT
useradd -m linda
useradd -m john
useradd -m anna 
groupadd team
groupadd randomgroup
usermod -aG team anna
SCRIPT


Vagrant.configure('2') do |config|
    
    # set default settings
    config.vm.box = "ubuntu/bionic64"
    config.vm.provider "virtualbox" do |vb|
        vb.memory = 2048
        vb.cpus = 1
    end

    config.vm.define :DevOps2, primary: true do |machine|
        machine.vm.host_name = "DevOps2.local"
        machine.vm.network "private_network", ip: "192.168.10.5"
        config.vm.provision "shell", inline: $useraddscript

        machine.vm.provider "virtualbox" do |vb|
            vb.cpus = 1
        end

        machine.vm.synced_folder "DevOps2/", "/home/vagrant/mission"
    end
end


