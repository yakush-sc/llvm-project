add_loader_object(
  crt1
  SRC
    start.cpp
  DEPENDS
    libc.config.linux.app_h
    libc.include.sys_mman
    libc.include.sys_syscall
    libc.src.__support.OSUtil.osutil
    libc.src.string.memcpy
  COMPILE_OPTIONS
    -fno-omit-frame-pointer
    -ffreestanding # To avoid compiler warnings about calling the main function.
)
