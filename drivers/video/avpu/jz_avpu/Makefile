# real (hardware) driver
obj-$(CONFIG_AVPU_DRIVER) += avpu.o
avpu-objs := avpu_main.o avpu_ip.o avpu_alloc.o avpu_alloc_ioctl.o

ifeq ($(CONFIG_AVPU_NO_DMABUF),1)
  avpu-objs += avpu_no_dmabuf.o
else
  avpu-objs += avpu_dmabuf.o
endif
