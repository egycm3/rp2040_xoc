add_executable(dhry1
        dhry1.c dhry_2.c
)

pico_enable_stdio_usb(dhry1 1)

pico_add_extra_outputs(dhry1)

target_link_libraries(dhry1 pico_stdlib)
