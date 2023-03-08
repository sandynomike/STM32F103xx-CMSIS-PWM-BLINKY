# STM32F103xx-CMSIS-PWM-BLINKY

This project contains the bare minimum code required to get a 1 Hz blinking LED on an STM32F103xx (Blue Pill).<br>
Requires the following for your OS, and the Path variable must be set to point to these binaries:<br>
The makefile will have to be edited as follows: The FLASHER path variable to the STM32_Programmer_CLI.exe file may have to be updated so that it points to the program in your system. Also, the FLASHPORT variable will have to be updated to to point to the COM port of the attached programmer.
Requires:<br>
<hr>
Editor of your choice<br>
arm-none-eabi-gcc toolchain<br>
make<br>
git-bash (for windows)<br>
STM32_Programmer_CLI.exe Program to upload .elf file to the microcontroller / Blue Pill<br>
<hr>
To compile, navigate to the directory containing main.c (using git-bash in Windows). If using LInux, rename Makefile.Linux to Makefile. Likewise, if using Windows, rename Makefile.Windows to Makefile. Then type 'make'. Assuming STM32CubeProgrammer is installed in the expected folder, make will also attempt to upload the code to the microcontroller, so, make sure it is connected and ready to accept code before performing the make command. Optionally, the .elf file can be uploaded manually as a separate process.
