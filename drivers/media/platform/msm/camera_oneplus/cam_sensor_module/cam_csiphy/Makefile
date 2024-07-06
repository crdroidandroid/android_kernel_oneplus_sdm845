ccflags-y += -Idrivers/media/platform/msm/camera_oneplus/cam_utils
ccflags-y += -Idrivers/media/platform/msm/camera_oneplus/cam_cpas/include
ccflags-y += -Idrivers/media/platform/msm/camera_oneplus/cam_sensor_module/cam_sensor_io
ccflags-y += -Idrivers/media/platform/msm/camera_oneplus/cam_sensor_module/cam_sensor_utils
ccflags-y += -Idrivers/media/platform/msm/camera_oneplus/cam_sensor_module/cam_cci
ccflags-y += -Idrivers/media/platform/msm/camera_oneplus/cam_req_mgr
ccflags-y += -Idrivers/media/platform/msm/camera_oneplus/cam_smmu/

CFLAGS_cam_csiphy_soc.o += $(call cc-disable-warning, fortify-source)
obj-$(CONFIG_SPECTRA_CAMERA) += cam_csiphy_soc.o cam_csiphy_dev.o cam_csiphy_core.o
