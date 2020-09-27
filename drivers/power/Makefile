obj-$(CONFIG_POWER_AVS)		+= avs/
obj-$(CONFIG_POWER_RESET)	+= reset/
obj-$(CONFIG_POWER_SUPPLY)	+= supply/
obj-$(CONFIG_ARCH_QCOM)          += qcom/
obj-$(CONFIG_TCPC_RT1711H)	+= rt-charger.o

ifdef CONFIG_MACH_ASUS_ZS661KS
obj-$(CONFIG_CHARGER_PCA9468)	+= pca9468_charger_zs661ks.o
else
obj-$(CONFIG_CHARGER_PCA9468)	+= pca9468_charger.o
endif