These files are from libc++, release 9.0.0.

tag: llvmorg-9.0.0
git: 0399d5a9682b3cef71c653373e38890c63c4c365

Update Instructions
-------------------

Run `system/lib/update_libcxx.py path/to/llvm-project`

Local Modification
------------------

Local modifications are marked with the comment: 'XXX EMSCRIPTEN'

1. Define _LIBCPP_OBJECT_FORMAT_ELF under __asmjs__ in libcxx/__config.

2. Define _LIBCPP_HAS_THREAD_API_PTHREAD in libcxx/__config./

3. Define _LIBCPP_ELAST in libcxx/include/config_elast.h

4. Set init_priority of __start_std_streams in libcxx/iostream.cpp
