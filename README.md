*** Here is a tools & stuff for building a kernel for a10s (physwizz kernel)! ***

- Clang (version: 9): https://github.com/samsung-mt6765-devs/clang-9
- GCC Linaro 7.5.0 (aarch64-linux-gnu) : https://github.com/samsung-mt6765-devs/aarch64-linux-gnu
- GCC (aarch64-linux-android) : https://github.com/samsung-mt6765-devs/aarch64-linux-android

Also you need to edit a Makefile in kernel/samsung/a10s, edit this lines: CROSS_COMPILE and CC, you can also use the build_kernel.sh script but u need to edit it (edit paths to toolchains)

To flash your builded kernel, you need a AnyKernel, you can get it from ItzKaguya or Starlix Kernel, took Image.gz-dtb from out/arch/arm64/boot/ and replace it, edit anykernel.sh (here you can edit the text when your kernel is flashing) and pack it to .zip archive

Good luck with building kernel!
