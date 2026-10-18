# BakaSU + SuSFS + BBG Kernel for A04s

Source is based on `SF` binary kernel.

# Download

Get them from [releases](https://github.com/lesdieuxx/android_kernel_a047f_bakasu/releases) or from the latest [Kernel build CI](https://github.com/lesdieuxx/android_kernel_a047f_bakasu/actions).

# Flashing

Recommended way is to flash AnyKernel3 zip files using recovery or system if you already have root.

`boot.img` modification is possible but, I don't release them. Do it yourself using [Android_boot_image_editor](https://github.com/cfig/Android_boot_image_editor).

# Building

Building is possible through two main ways. One is forking and using Github Actions. I added them to repository but for a release build I use my local machine to compile.

For local building you need `clang-r596125` from [AOSP](https://android.googlesource.com/platform/prebuilts/clang/host/linux-x86/+/refs/heads/main-kernel).
(Sparse-checkout example is available in Github workflow [build.yml](https://github.com/lesdieuxx/android_kernel_a047f_bakasu/blob/master/.github/workflows/build.yml))
After downloading clang toolchain, add `bin` directory to PATH and run the `build_kernel.sh` script.
