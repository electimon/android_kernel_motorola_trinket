focaltech_0flash_mmi-y += focaltech_core.o
focaltech_0flash_mmi-y += focaltech_esdcheck.o
focaltech_0flash_mmi-y += focaltech_ex_fun.o
focaltech_0flash_mmi-y += focaltech_ex_mode.o
focaltech_0flash_mmi-y += focaltech_flash.o
focaltech_0flash_mmi-y += focaltech_gesture.o
focaltech_0flash_mmi-y += focaltech_point_report_check.o
focaltech_0flash_mmi-y += focaltech_test/focaltech_test.o
focaltech_0flash_mmi-y += focaltech_test/focaltech_test_ini.o

focaltech_0flash_mmi-y += focaltech_test/supported_ic/focaltech_test_ft8756.o
focaltech_0flash_mmi-y += focaltech_flash_ft8756.o
focaltech_0flash_mmi-y += focaltech_spi_v1_1_1.o

ifneq ($(filter m y,$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI_ENABLE_DOUBLE_TAP)),)
	ccflags-y += -DFOCALTECH_SENSOR_EN
endif
ifneq ($(filter m y,$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI_ENABLE_PALM)),)
	ccflags-y += -DFOCALTECH_PALM_SENSOR_EN
endif

obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI) += focaltech_0flash_mmi.o
