Vagrant::Config.run do |config|
  config.vm.box = "lucid32"
  config.vm.box_url = "http://files.vagrantup.com/lucid32.box"
  config.vm.boot_mode = :gui

  config.vm.provision :chef_solo do |chef|
    chef.recipe_url = "http://files.vagrantup.com/getting_started/cookbooks.tar.gz"
    chef.add_recipe("vagrant_main")
  end
end

