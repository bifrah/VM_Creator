# VM_Creator
# A simple script to create a VM


0 - Changer le chemin machine folder  de vagrant pour eviter de remplir ton home, donc soit dans tmp. soit dans ton server goinfre

Pour check le chemin de creation de la VM :
VBoxManage list systemproperties | grep "Default machine folder:"

Pour le changer :
	vboxmanage setproperty machinefolder ${PATH_OF_VM}
Pour tmp :	vboxmanage setproperty machinefolder /tmp

1 - Creer un fichier nomme Vagrantfile a la racine de ton repo et copier le code dedans.

2 - Run la command :
	'vagrant plugin install vagrant-reload'

3 - Lancer vagrant :
	'vagrant up'

4 - Attendre 5 ou 10min.

5 - Pour lancer un terminal en local qui fera tout dans la VM :
	'vagrant ssh'