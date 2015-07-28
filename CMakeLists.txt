add_executable(bootinfo src/main.c)

target_link_libraries(bootinfo
    libsel4
    libsel4printf
    libsel4startstop
)

add_dependencies(bootinfo sel4_kernel)
