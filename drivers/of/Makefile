subdir-ccflags-y += 

obj-y = base.o device.o platform.o
obj-$(CONFIG_OF_DYNAMIC) += dynamic.o
obj-$(CONFIG_OF_FLATTREE) += fdt.o
obj-$(CONFIG_OF_EARLY_FLATTREE) += fdt_address.o
obj-$(CONFIG_OF_PROMTREE) += pdt.o
obj-$(CONFIG_OF_ADDRESS)  += address.o
obj-$(CONFIG_OF_IRQ)    += irq.o
obj-$(CONFIG_OF_NET)	+= of_net.o
obj-$(CONFIG_OF_SELFTEST) += of_selftest.o
of_selftest-objs := selftest.o testcase-data/testcases.dtb.o
obj-$(CONFIG_OF_MDIO)	+= of_mdio.o
obj-$(CONFIG_OF_PCI)	+= of_pci.o
obj-$(CONFIG_OF_PCI_IRQ)  += of_pci_irq.o
obj-$(CONFIG_OF_MTD)	+= of_mtd.o
obj-$(CONFIG_OF_RESERVED_MEM) += of_reserved_mem.o
obj-$(CONFIG_OF_RESOLVE)  += resolver.o

CFLAGS_fdt.o = -I$(src)/../../scripts/dtc/libfdt
CFLAGS_fdt_address.o = -I$(src)/../../scripts/dtc/libfdt
ccflags-y += -I$(srctree)/drivers/misc/mediatek/include
