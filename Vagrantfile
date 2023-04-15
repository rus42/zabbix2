# -*- mode: ruby -*-
# vi: set ft=ruby :
virt_machines=[
    { :hostname => "zabbixagent1" ,:ip => "192.168.0.20" },
    { :hostname => "zabbixagent2" ,:ip => "192.168.0.21" } ]
Vagrant .configure( "2") do |config |
        virt_machines.each do |machine |
            config.vm.box = "generic/ubuntu2004"
            config.vm.define machine[:hostname] do |node|
                node.vm.hostname = machine[:hostname]
                node.vm.network :public_network, bridge: "Intel(R) Wireless-AC 9560" , ip: machine[:ip]
                node.vm.provider "virtualbox" do |current_vm , override |
                    current_vm.name = machine[:hostname]
                    current_vm.gui = false
                    current_vm.memory = "512"
                    current_vm.cpus = 1
                    override.vm.provision "shell" , path: 'zabbix-agent.sh' , args: [ 'zabbix' , '123' , 'false' , machine[:hostname], machine[:ip], '192.168.1.120' ], run: "once"
                end
            end
        end
    end