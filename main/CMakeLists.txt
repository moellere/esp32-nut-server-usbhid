idf_component_register(SRCS "esp32-nut-server-usbhid.c"
                       INCLUDE_DIRS ".")

target_compile_definitions(${COMPONENT_LIB} PRIVATE
    "CONFIG_EXAMPLE_WIFI_SSID=\"${WIFI_SSID}\""
    "CONFIG_EXAMPLE_WIFI_PASSWORD=\"${WIFI_PASSWORD}\""
)
