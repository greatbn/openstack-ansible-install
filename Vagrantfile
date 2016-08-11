VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do | config |
	config.vm.box = "ubuntu/trusty64"
  config.vm.provider "virtualbox" do | vb |
    vb.memory = 4096
    vb.cpus =  2
  end
	config.vm.define "controller" do | m |
		m.vm.network :private_network, ip: "10.5.0.21"
		m.vm.network :public_network, bridge: "wlp3s0",
			use_dhcp_assigned_default_route: true
		m.vm.hostname = "controller"
	end

	config.vm.define "compute-1" do | n1 |
                n1.vm.network :private_network, ip: "10.5.0.22"
                n1.vm.hostname = "compute-1"
        end

end
