VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

    config.vm.box     = "ubuntu_1404_amd64"
    config.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box"

    config.vm.network "forwarded_port", guest: 80, host: 9090
    config.vm.network "forwarded_port", guest: 4200, host: 4200

    config.vm.provision "shell", path: "provisioning.sh"
end
