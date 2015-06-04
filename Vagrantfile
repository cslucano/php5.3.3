Vagrant.configure(2) do |config|
#  # A standard CentOS 6.5 x64 base install
#  config.vm.box = "chef/centos-6.5"
#  # A standard CentOS 7.0 install
#  config.vm.box = "chef/centos-7.0"
#  # A standard CentOS 6.6 x64 base install
#  config.vm.box = "chef/centos-6.6"
#  # A standard Fedora 20 x64 base install
#  config.vm.box = "chef/fedora-20"
   config.vm.box = "chef/centos-6.6"

   config.vm.network :private_network, ip: "192.168.33.10"
   config.vm.synced_folder "./", "/var/www/html", type: "nfs"


   config.vm.provision "ansible" do |ansible|
     ansible.playbook = "ansible/playbook.yml"
   end
end
