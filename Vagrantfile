Vagrant.configure("2") do |config|

  config.vm.define "centos7" do |centos7|
    centos7.vm.box = "centos/7"
    centos7.vm.provider :libvirt do |domain|
      domain.memory = 2048
      domain.cpus = 1
    end

    centos7.vm.provision "shell",
      inline: "yum install -y epel-release"
  end

  config.vm.define "rhel8" do |rhel8|
    rhel8.vm.box = "generic/rhel8"
    rhel8.vm.provider :libvirt do |domain|
      domain.memory = 2048
      domain.cpus = 1
    end
  end

end
