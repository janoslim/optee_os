# OP-TEE Trusted OS
This git contains source code for the secure side implementation of OP-TEE
project.

All official OP-TEE documentation has moved to http://optee.readthedocs.io.

// OP-TEE core maintainers

This is a modifided version of 3.7.0 tag from linaro. We are building it only
on rockchip SoCs. The command to build it i.e. on rk3399 platform is below:

make CFG_ARM64_core=y CFG_TEE_BENCHMARK=n CFG_TEE_CORE_LOG_LEVEL=2 \
     CROSS_COMPILE=aarch64-linux-gnu- CROSS_COMPILE_core=aarch64-linux-gnu- \
     CROSS_COMPILE_ta_arm32=arm-linux-gnueabihf- CROSS_COMPILE_ta_arm64=aarch64-linux-gnu- \
     O=out/arm PLATFORM=rockchip-rk3399

// Softgent core team
