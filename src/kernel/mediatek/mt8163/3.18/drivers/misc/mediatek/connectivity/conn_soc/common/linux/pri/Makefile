MTK_PLATFORM := $(subst ",,$(CONFIG_MTK_PLATFORM))
ifeq ($(CONFIG_MTK_COMBO), y)
ccflags-y += -I$(src)/../../linux/include \
						 -I$(src)/../../linux/pri/include \
						 -I$(src)/../../core/include \
						 -I$(src)/../../include \
						 -I$(src)/../ \
						 -I$(srctree)/drivers/misc/mediatek/btif/common/inc \
						 -I$(srctree)/drivers/misc/mediatek/connectivity/common_detect \
                         -I$(src)/../include

ccflags-y += -I$(srctree)/drivers/misc/mediatek/mach/$(MTK_PLATFORM)/include/mach

ccflags-y += -DWMT_CREATE_NODE_DYNAMIC=1
obj-y += stp_btif.o \
         stp_dbg.o \
         stp_exp.o \
         wmt_dev.o \
         wmt_exp.o

endif
