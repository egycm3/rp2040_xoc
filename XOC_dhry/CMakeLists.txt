add_executable(dhry1_xoc
        dhry1.c dhry_2.c
)

pico_enable_stdio_usb(dhry1_xoc 1)

target_link_libraries(dhry1_xoc pico_stdlib hardware_clocks)

pico_add_extra_outputs(dhry1_xoc)

#pico_set_binary_type(dhry1_xoc copy_to_ram)
