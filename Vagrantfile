Vagrant.configure("2") do |config|
    config.vm.box = 'bento/ubuntu-16.04'
    config.ssh.insert_key = false
    config.vm.define('dot') do |t|
        t.vm.hostname = 'dot'
        t.vm.network(:private_network, ip: '192.168.42.42')
    end
end
