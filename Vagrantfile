Vagrant.configure("2") do |config| 
  config.vm.boot_timeout = 1200 # 20 minutes
  config.vm.box = "ubuntu/focal64" # Ubuntu 20.04 LTS

  config.vm.network "forwarded_port", guest: 3000, host: 3000 # Port forwarding

  config.vm.provider "virtualbox" do |vb| # VirtualBox specific settings
    vb.name = "assignment3" # VM name
    vb.memory = "8192" # 8GB
  end
  
  config.vm.cloud_init content_type: "text/cloud-config", path: "cloud-init.yaml" # Cloud-init configuration
end
