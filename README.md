# VM_Creator
# A simple script to create a VM

Le script sert a checker si la version de vagrant utilise est la derniere.

0 - Changer le chemin machine folder  de vagrant pour eviter de remplir ton home, donc soit dans tmp. soit dans ton server goinfre

Pour check le chemin de creation de la VM :
	VBoxManage list systemproperties | grep "Default machine folder:"

Pour le changer :
	vboxmanage setproperty machinefolder ${PATH_OF_VM}
Pour tmp :	vboxmanage setproperty machinefolder /tmp

1 - Run la command :
	'vagrant plugin install vagrant-reload'

2 - Lancer vagrant :
	'vagrant up'

3 - Attendre 5 ou 10min.

4 - Pour lancer un terminal en local qui fera tout dans la VM :
	'vagrant ssh'