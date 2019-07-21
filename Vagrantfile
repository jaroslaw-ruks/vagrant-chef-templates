Vagrant.configure("2") do |config|

  config.vm.box = "debian/stretch64"
  config.vm.provision "chef_solo" do |chef|
  	chef.arguments = "--chef-license accept"
    chef.cookbooks_path = "../chef-repo/"
    chef.add_recipe "bootstrap"
	end
end
