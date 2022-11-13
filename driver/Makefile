obj-m = rx666m.o

ccflags-y += -Wall -g -I$(PWD)/../common/

KVERSION = $(shell uname -r)
all:
	make -C /lib/modules/$(KVERSION)/build M=$(PWD) modules
clean:
	make -C /lib/modules/$(KVERSION)/build M=$(PWD) clean


