# Infineon's fork of OpenOCD

This project came from Infineon's customized [openocd](https://github.com/Infineon/modustoolbox-software/issues/5)


## Usage

In shell, execute:


```bash
.\openocd.exe -s ..\share\openocd\ -f scripts\interface\kitprog3.cfg -f target/psoc4.cfg -c "set PSOC4_USE_ACQUIRE 0; kitprog3 power_config on 3300; init; sleep 1000; program foo.hex; shutdown"

```

