# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/amazonlinux-2"

  hosts = %w(node1 node2)

  hosts.each do |host|
    config.vm.define host do |c|
      c.vm.hostname = host
      c.vm.synced_folder "./sync", "/sync"
    end
  end
end
