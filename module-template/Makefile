obj-m   += module-template.o

#KDIR    := /lib/modules/$(shell uname -r)/build
KDIR    := /home/ubuntu/qemu/linux
PWD     := $(shell pwd)

default:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) modules

clean:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) clean
	rm -f modules.order

