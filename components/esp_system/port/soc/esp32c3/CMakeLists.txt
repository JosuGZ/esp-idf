set(srcs "clk.c"
         "reset_reason.c"
         "../../async_memcpy_impl_gdma.c"
         "apb_dma.c"
         "../../arch/riscv/panic_arch.c")
add_prefix(srcs "${CMAKE_CURRENT_LIST_DIR}/" ${srcs})

target_sources(${COMPONENT_LIB} PRIVATE ${srcs})
