idf_component_register(
	SRCS
		"main.c"
	PRIV_REQUIRES
		esp_lcd
		esp_driver_i2s
		esp_timer
		nvs_flash
		badge-bsp
	INCLUDE_DIRS
		"."
)

idf_build_set_property(COMPILE_OPTIONS "-Wno-error=unused-variable" APPEND)
idf_build_set_property(COMPILE_OPTIONS "-Wno-error=unused-const-variable" APPEND)
