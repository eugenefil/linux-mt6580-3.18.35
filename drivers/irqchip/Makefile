subdir-ccflags-y += 

obj-$(CONFIG_IRQCHIP)			+= irqchip.o

obj-$(CONFIG_ARCH_BCM2835)		+= irq-bcm2835.o
obj-$(CONFIG_ARCH_EXYNOS)		+= exynos-combiner.o
obj-$(CONFIG_ARCH_HIP04)		+= irq-hip04.o
obj-$(CONFIG_ARCH_MMP)			+= irq-mmp.o
obj-$(CONFIG_ARCH_MVEBU)		+= irq-armada-370-xp.o
obj-$(CONFIG_ARCH_MXS)			+= irq-mxs.o
obj-$(CONFIG_ARCH_S3C24XX)		+= irq-s3c24xx.o
obj-$(CONFIG_DW_APB_ICTL)		+= irq-dw-apb-ictl.o
obj-$(CONFIG_METAG)			+= irq-metag-ext.o
obj-$(CONFIG_METAG_PERFCOUNTER_IRQS)	+= irq-metag.o
obj-$(CONFIG_ARCH_MOXART)		+= irq-moxart.o
obj-$(CONFIG_CLPS711X_IRQCHIP)		+= irq-clps711x.o
obj-$(CONFIG_OR1K_PIC)			+= irq-or1k-pic.o
obj-$(CONFIG_ORION_IRQCHIP)		+= irq-orion.o
obj-$(CONFIG_OMAP_IRQCHIP)		+= irq-omap-intc.o
obj-$(CONFIG_ARCH_SUNXI)		+= irq-sun4i.o
obj-$(CONFIG_ARCH_SUNXI)		+= irq-sunxi-nmi.o
obj-$(CONFIG_ARCH_SPEAR3XX)		+= spear-shirq.o
obj-$(CONFIG_ARM_GIC)			+= irq-gic.o irq-gic-common.o
obj-$(CONFIG_ARM_GIC_V3)		+= irq-gic-v3.o irq-gic-common.o
obj-$(CONFIG_ARM_NVIC)			+= irq-nvic.o
obj-$(CONFIG_ARM_VIC)			+= irq-vic.o
obj-$(CONFIG_ATMEL_AIC_IRQ)		+= irq-atmel-aic-common.o irq-atmel-aic.o
obj-$(CONFIG_ATMEL_AIC5_IRQ)	+= irq-atmel-aic-common.o irq-atmel-aic5.o
obj-$(CONFIG_IMGPDC_IRQ)		+= irq-imgpdc.o
obj-$(CONFIG_SIRF_IRQ)			+= irq-sirfsoc.o
obj-$(CONFIG_RENESAS_INTC_IRQPIN)	+= irq-renesas-intc-irqpin.o
obj-$(CONFIG_RENESAS_IRQC)		+= irq-renesas-irqc.o
obj-$(CONFIG_VERSATILE_FPGA_IRQ)	+= irq-versatile-fpga.o
obj-$(CONFIG_ARCH_NSPIRE)		+= irq-zevio.o
obj-$(CONFIG_ARCH_VT8500)		+= irq-vt8500.o
obj-$(CONFIG_TB10X_IRQC)		+= irq-tb10x.o
obj-$(CONFIG_XTENSA)			+= irq-xtensa-pic.o
obj-$(CONFIG_XTENSA_MX)			+= irq-xtensa-mx.o
obj-$(CONFIG_IRQ_CROSSBAR)		+= irq-crossbar.o
obj-$(CONFIG_BRCMSTB_L2_IRQ)		+= irq-brcmstb-l2.o \
					   irq-bcm7120-l2.o
obj-$(CONFIG_KEYSTONE_IRQ)		+= irq-keystone.o
obj-$(CONFIG_ARCH_MEDIATEK)		+= irq-mtk-sysirq.o

# Mediatek solution: GIC & EIC
MTK_PLATFORM := $(subst ",,$(CONFIG_MTK_PLATFORM))
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include/mt-plat/$(MTK_PLATFORM)/include

obj-$(CONFIG_MTK_GIC)                   += irq-mt-gic.o
obj-$(CONFIG_MTK_EIC)                   += irq-mt-eic.o
obj-$(CONFIG_MTK_INTPOL)		+= irq-mtk-intpol.o

ifeq ($(CONFIG_MT_ENG_BUILD),y)
CFLAGS_irq-mt-gic.o := -DDEBUG
CFLAGS_irq-mt-eic.o := -DDEBUG
endif
