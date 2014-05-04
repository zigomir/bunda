require 'yaml'

CONF = YAML.load_file('server_config.yml')

Vagrant.configure('2') do |config|
  config.vm.box = 'ubuntu/trusty64'

  CONF['forward_ports'].each do |port|
    config.vm.network :forwarded_port, guest: port['guest'], host: port['host']
  end

  config.vm.synced_folder '.', '/vagrant', type: 'nfs'
  config.vm.network :private_network, ip: CONF['private_ip']

  config.vm.provider :virtualbox do |provider, override|
    provider.customize ['modifyvm', :id, '--name',   CONF['name']]
    provider.customize ['modifyvm', :id, '--memory', CONF['memory']]
  end
end