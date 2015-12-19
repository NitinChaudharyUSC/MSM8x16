The files shared in this repository show case some of the work done by me while working for Samsung Research Institute - Bangalore, India a part of Samsung Electronics (Mobile Communicatons Division). The work presented is only the part of my work that has been released by Samsung Opensource Release Centre, though the work done in BSP(Board Support Package) layer in Secondary Bootloader 1 (SBL1) and Little Kernel (LK) (Both being Qualcomm's Propreitary code) cannot be opensource due to legal issues. The code shared here is relevant to one of two major backbone chipsets used in Samsung for Midrange Price Mobile Devices Like Galaxy Tab4, Galaxy Grand2 and Galaxy A5/A3 series. The following is a small summary of both:

MSM8x26/MSM8x28: A 28nm SoC consisting of four ARM Cortex A7 CPUs (32 bits) running at (1.2 GHz) alongside an Adreno 305 GPU. With MSM8x28 it was able to clock upto 1.4GHz and supported LPDDR3 as well.

MSM8x16: A 28nm SoC consisting of four ARM Cortex A53 CPUs (64 bits) capable of clocking to 1.4GHz alongside an Adreno 306 GPU with support for LPDDDR3/SDRAM.

Kindly follow the below guide to see the work done:

A. Linux Device Driver:
  1. MicroUSB IC SM5504: drivers/misc/sm5504.c
  2. MicroUSB IC SM5502: drivers/misc/sm5502.c
  3. MiscroUSB IC TSU6721: drivers/misc/tsu6721.c
  4. MicroUSB IC MAX77843: drivers/extcon/extcon-max77849
  5. MicroUSB IC MAX7749: drivers/extcon/extcon-max77843

B. Device Trees for MSM8x26/MSM8x28 Chipsets: Peek into the directory arch/arm/boot/dts/samsung/msm8x26/

C. Work on devfreq Subsystem for Bus Bandwidth Prediction and Management (Opensource Release Awaited)

D. Work on cpufreq subsystem for integrating Scheduler with cpufreq Governor (Opensource Release Awaited)
