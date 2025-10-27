ccflags-y += -DCONFIG_TOUCHSCREEN_JADARD_DEBUG=y
ccflags-y += -DCONFIG_TOUCHSCREEN_JADARD_SORTING=y

ifeq ($(TARGET_BUILD_VARIANT), user)
	ccflags-y += -D__JADARD_GKI__
endif

##### Makefile for the Jadard touchscreen drivers.####
ccflags-y += -D__JADARD_KMODULE__

jadard_touch-objs := jadard_module.o
jadard_touch-objs += jadard_ic_JD9365TL.o
jadard_touch-objs += jadard_common.o jadard_platform.o
jadard_touch-objs += jadard_debug.o
jadard_touch-objs += jadard_sorting.o
obj-y += jadard_touch.o
