add_executable(XOC
        XOC.c
        )

pico_enable_stdio_usb(XOC 1)

pico_set_binary_type(XOC copy_to_ram)

target_link_libraries(XOC pico_stdlib hardware_clocks hardware_pll)

pico_add_extra_outputs(XOC)

