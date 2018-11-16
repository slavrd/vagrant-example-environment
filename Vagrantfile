Vagrant.configure("2") do |config|

  (1..2).each do |i|
    vm_name="web%02d" % [i]
    config.vm.define vm_name do |web|
      web.vm.box = "slavrd/nginx64"
      web.vm.hostname = vm_name
    end
  end

  config.vm.define "mysql" do |db|
    db.vm.box = "slavrd/mysql64"
    db.vm.hostname = "mysql"
  end

end
