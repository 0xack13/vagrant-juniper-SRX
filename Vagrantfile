Vagrant.configure(2) do |config|
  config.vm.box = "juniper/ffp-12.1X47-D15.4-packetmode"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 512
    vb.cpus = 2
    vb.gui = false
  end

  config.vm.define "r1" do |r1|
    r1.vm.host_name = "r1"
    r1.vm.network "private_network",
                     ip: "192.168.1.1",
                     virtualbox__intnet: "1-2"
  end

  config.vm.define "r2" do |r2|
    r2.vm.host_name = "r2"
    r2.vm.network "private_network",
                     ip: "192.168.1.2",
                     virtualbox__intnet: "1-2"
  end
end
