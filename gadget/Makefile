KERNEL_PATH ?= /lib/modules/`uname -r`/build


g_ipod-y := ipod.o
obj-m += g_ipod.o

ccflags-y += -DDEBUG
ccflags-y += -DVERBOSE_DEBUG
ccflags-y += -I$(src)

all:
	make -C $(KERNEL_PATH) M=$(PWD) modules

clean:
	make -C $(KERNEL_PATH) M=$(PWD) clean

