sch_netem:
	# Install module
	- sudo mkdir -p /lib/modules/$(uname -r)/kernel/net/sched
	sudo cp sch_netem.ko /lib/modules/$(uname -r)/kernel/net/sched
	echo 'sch_netem' | sudo tee -a /etc/modules
	sudo depmod
	# Load module for current run as well
	sudo insmod sch_netem.ko