Vagrant.configure("2") do |config|
 
#  config.vm.provider "virtualbox" do |v|
#    v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
#    v.customize ["modifyvm", :id, "--natdnsproxy1", "on"]
#  end

# creating a virtual machine ubuntu
 config.vm.box = "ubuntu/xenial64"

# assign private ip to our VM
 config.vm.network "private_network", ip: "192.168.10.100"

# ensure to install hostupdater plugin in our local host before rerunning the vagrant
# config.hostsupdater.aliases = ["development.local"]

# Sync folder from OS to VM
               # "." means current location -  into/inside VM
 config.vm.synced_folder ".", "/home/vagrant/app"          

end

