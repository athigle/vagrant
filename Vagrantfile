Vagrant.configure("2") do |config|

#COnfiguring Ubuntu
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "ubuntu/trusty64"
    ubuntu.vm.hostname = "ubuntu-avani"
    ubuntu.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)", type: "dhcp"
    ubuntu.vm.network "forwarded_port", guest: 80, host:8082
  end

#configuring CentOS
  config.vm.define "centos" do |centos|
    centos.vm.box = "centos/7"
    centos.vm.hostname = "centos-avani"
    centos.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)", type: "dhcp"
    centos.vm.network "forwarded_port", guest: 80, host:8083
  end

end
