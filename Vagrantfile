Vagrant.configure("2") do |config|
    config.vm.define 'setupserver01' do |config|
        config.vm.box = 'ubuntu/trusty64'
        config.vm.hostname = 'setupserver01'
        config.vm.synced_folder '.', '/vagrant', disabled: true
        config.vm.network :forwarded_port, guest: 22, host: 2232, id: "ssh", auto_correct: false
    end
end
