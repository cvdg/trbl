# trbl  - tribble


sudo aptitude install build-essential libvirt-dev golang

git clone https://github.com/dmacvicar/terraform-provider-libvirt.git

export CGO_ENABLED="1"
make

mkdir -p ~/.local/share/terraform/plugins/registry.terraform.io/dmacvicar/libvirt/0.6.2/linux_amd64
cp -pv terraform-provider-libvirt ~/.local/share/terraform/plugins/registry.terraform.io/dmacvicar/libvirt/0.6.2/linux_amd64

