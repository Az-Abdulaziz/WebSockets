
1. Install rosetta

/usr/sbin/softwareupdate --install-rosetta --agree-to-license

2. Install vagrant with homebrew

brew install vagrant

3. Create an account on vmware

customerconnect.vmware.com 79

4. Download & Install VMWare Fusion Tech Preview

download page 161

5. Create link

ln -s /Applications/VMWare\ Fusion\ Tech\ Preview.app /Applications/VMWare\ Fusion.app

6. Install vmware provider

install vagrant

7. Install Plugin

vagrant plugin install vagrant-vmware-desktop

8. Create a Vagrantfile in a folder with below content

Vagrant.configure(“2”) do |config|

config.vm.box = “spox/ubuntu-arm”

config.vm.box_version = “1.0.0”
end

9. Bring up vm

Go to the folder where you created Vagrantfile & issue below command.

vagrant up

vagrant ssh

exit

vagrant halt

vagrant destroy

10. Create fedora vm (equivalent to centos)

mkdir -p ~/vms/fedora

cd ~/vms/fedora

vagrant init jacobw/fedora35-arm64

vagrant up

vagrant ssh

exit

vagrant halt

vagrant destroy

