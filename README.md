# Learning Rust through embedded projects

Going through [The Embedded Rust Book](https://docs.rust-embedded.org/book/).

## Tools
1. [STM32F404 Discovery kit](https://www.st.com/en/evaluation-tools/stm32f4discovery.html)

## Set up
1. Setting udev rules

``` 
# Bus 001 Device 016: ID 0483:374b STMicroelectronics ST-LINK/V2.1
ATTRS{idVendor}=="0483", ATTRS{idProduct}=="374b", TAG+="uaccess"
```

1. Open OCD
```sh
openocd -f interface/stlink.cfg -f target/stm32f4x.cfg
```

