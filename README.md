# Dependencies:
- `arm-none-eabi-newlib`
- `arm-none-eabi-gcc`
- `make`
# And for flashing the binary to the microcontroller:
- `st-link commandline tools`
# Procedure(run these command):
1. `$ make` compile the project
2. `$ st-info --probe` if device is successfully listed that means device is connected to the pc
3. `$ st-flash write build/blink.bin 0x8000000` flash the image
