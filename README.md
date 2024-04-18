# Lora with STM32 B-L072Z-LRWAN1

This repository contains code and configurations for the STM32 B-L072Z-LRWAN1.

---

## Requirements
- STM32 Cube MX for code generation
- VSCode with extension:
  - stm32-for-vscode 
  - cortex-debug

For stm32-for-vscode, you can either do the automatic installation as described in the extension page or manually install the following tools.
- [GNU Arm Embedded Toolchain](https://developer.arm.com/open-source/gnu-toolchain/gnu-rm/downloads)
- OpenOCD [Windows](https://gnutoolchains.com/arm-eabi/openocd/), [Other Platforms](https://xpack.github.io/dev-tools/openocd/install/)


## Usage

1. Clone the repository
2. Open the project (*.ioc file) in STM32 Cube MX
3. Press Generate Code
4. Open the project folder that contains the .ioc in VSCode (e.g. `stm-lora-test`)
5. Press F5 to build and debug

Important: Generate Code overwrites all parts in the code that are not between `USER CODE BEGIN` and `USER CODE END` comments!
