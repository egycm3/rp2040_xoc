add_executable(CLOCK_STAT
        CLOCK_STAT.c
        )

pico_enable_stdio_usb(CLOCK_STAT 1)

target_link_libraries(CLOCK_STAT pico_stdlib hardware_clocks)

pico_add_extra_outputs(CLOCK_STAT)
