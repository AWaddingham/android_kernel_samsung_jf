GCC_VERSION      := $(shell $(CONFIG_SHELL) $(PWD)/scripts/gcc-version.sh $(CROSS_COMPILE)gcc)

ifeq ($(CONFIG_MSM_CAMERA_V4L2),y)
  EXTRA_CFLAGS += -Idrivers/media/video/msm-jf
  EXTRA_CFLAGS += -Idrivers/media/video/msm-jf/io
  EXTRA_CFLAGS += -Idrivers/media/video/msm-jf/csi
  EXTRA_CFLAGS += -Idrivers/media/video/msm-jf/eeprom
  EXTRA_CFLAGS += -Idrivers/media/video/msm-jf/sensors
  EXTRA_CFLAGS += -Idrivers/media/video/msm-jf/actuators
  obj-$(CONFIG_MSM_CAMERA)   += msm_cam_server.o
endif
