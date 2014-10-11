Vagrant.configure("2") do |config|
  config.vm.box = 'vsphere'
  config.vm.box_url = 'https://vagrantcloud.com/ssx/boxes/vsphere-dummy/versions/1/providers/vsphere.box'

  config.vm.provider :vsphere do |vsphere|
    # The host we're going to connect to
    vsphere.host = 'vserver.host.tld'                            

   # The host for the new VM
    vsphere.compute_resource_name = 'esxi.host.tld'            

    # The resource pool for the new VM
    vsphere.resource_pool_name = 'My Resource Pool'                    

    # The template we're going to clone        
    vsphere.template_name = 'virtual-machine-template'    

    # The name of the new machine
    vsphere.name = 'new-server.host.tld'                                     

    # vSphere login
    vsphere.user = 'root'                                    

    # vSphere password
    vsphere.password = 'password'                            

    # If you don't have SSL configured correctly, set this to 'true'
    vsphere.insecure = true                                    
  end
end
