
ifneq ($(MTK_ROOT_BUILD),)

    include $(MTK_ROOT_BUILD)/Makefile
else

endif

ifeq ($(CONFIG_TRUSTONIC_TEE_SUPPORT),y)


    ccflags-y += -I$(srctree)/drivers/misc/mediatek/mach/$(MTK_PLATFORM)/include/trustzone/utils/tlutils
include $(srctree)/drivers/misc/mediatek/gud/Makefile.include
    obj-y += secwidevinemdw.o
endif
