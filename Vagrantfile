Vagrant.configure(2) do |config|

  config.vm.define "my-develop" do |develop|
    develop.vm.box = 'CentOS-6.6-x86_64'
    develop.vm.box_url = "https://developer.nrel.gov/downloads/vagrant-boxes/CentOS-6.6-x86_64-v20150426.box"
    develop.vm.network :private_network, ip: "10.99.99.99"
    develop.vm.synced_folder ".", "/vagrant", type: "nfs"
    develop.vm.network :forwarded_port, host: 8081, guest: 80

    develop.vm.provision :ansible do |vm|
      vm.playbook = 'site.yml'
    end
  end
end