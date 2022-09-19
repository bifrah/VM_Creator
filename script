#!/bin/sh

set -eu

VAGRANT="https://releases.hashicorp.com/vagrant/2.2.19/vagrant_2.2.19_linux_amd64.zip"

mkdir -p ~/bin
wget -qO- "$VAGRANT" | busybox unzip -d ~/bin/ - 1> /dev/null
chmod +x ~/bin/vagrant
vagrant autocomplete install 1> /dev/null
vagrant version