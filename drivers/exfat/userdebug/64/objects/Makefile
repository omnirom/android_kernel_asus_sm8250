# Rules for making the exFAT driver.
#
# Copyright (c) 2009-2016 Anton Altaparmakov & Tuxera Inc. All rights reserved.
#
# You can set various options for the exFAT driver here:

CONFIG_EXFAT_NAME = texfat

ifeq ($(wildcard include/linux/compile.h include/generated/compile.h),)
EXTRA_CFLAGS += -DTUXERA_NO_COMPILE_H -DUTS_MACHINE=\"$(UTS_MACHINE)\"
ifdef CONFIG_SMP
SMP=SMP
endif
ifdef CONFIG_PREEMPT
PREEMPT=preempt
endif
EXTRA_CFLAGS += -DUTS_VERSION=\"$(SMP)\ $(PREEMPT)\ UNKNOWN\"
endif

obj-m += $(CONFIG_EXFAT_NAME).o

$(CONFIG_EXFAT_NAME)-objs := texfat.o
