Vagrant.configure("2") do |config|
  ENV['VAGRANT_DEFAULT_PROVIDER'] = 'docker'
  config.vm.provider "docker" do |d|
    d.image = "monkeyswithbuttons/docker-vagrant-centos7"
    d.has_ssh = true
    d.create_args = [ "--privileged", "-v", "/sys/fs/cgroup:/sys/fs/cgroup:ro" ]
  end
end
