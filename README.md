# nRF91TCPHTTPSToServerTest

## Test BSD library - NB-IoT TCP HTTPS client connect to nRF91ServerTest

### Application Description
    curl Test 
    # curl --cacert cert/nrftestserver.cer https://139.162.251.115:42512
    # {"ActionName":"BSDTest","LED1":false,"LED2":true}


    Client: Connect to nRF91ServerTest
    Client: Parse JSON and toggel LED's  
    Client: Close socket

### Test Server 
    # Test Server
    CONFIG_SERVER_HOST="139.162.251.115"
    CONFIG_SERVER_PORT=42512

### See diff in commit files to illustrate how http via TLS was enabled in code: 

https://github.com/FrancisSieberhagen/nRF91TCPHTTPSToServerTest/commit/685e69267462bd5c0278532b020a0442e0ff5c13

### Build hex 
    $ export ZEPHYR_BASE=/????
    $ west build -b nrf9160_pca10090ns

### Program nRF9160-DK using nrfjprog
    $ nrfjprog --program build/zephyr/merged.hex -f nrf91 --chiperase --reset --verify

### nRF Connect
![alt text](https://raw.githubusercontent.com/FrancisSieberhagen/nRF91TCPHTTPToServerTest/master/images/nRFConnect.jpg)

### nRF Connect SDK!
    https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/index.html

    Installing the nRF Connect SDK through nRF Connect for Desktop
    https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/gs_assistant.html

### Nordicsemi nRF9160 NB-IoT 
    https://www.nordicsemi.com/Software-and-tools/Development-Kits/nRF9160-DK

### CLion - A cross-platform IDE for C
    https://devzone.nordicsemi.com/f/nordic-q-a/49730/howto-nrf9160-development-with-clion

### Good place to get started/installed and start learning:
https://devzone.nordicsemi.com/nordic/nrf-connect-sdk-guides/b/getting-started/posts/nrf-connect-sdk-tutorial

### NRF Getting Started
https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/getting_started.html#getting-started
https://infocenter.nordicsemi.com/pdf/nRF9160_DK_Getting_Started_Guide_v1.1.pdf

### NRF Connect SDK Documentation
https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/introduction.html

### Make sure to understand Kconfig
See most Kconfig configuration documented here:
https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/kconfig/index-all.html

### Make sure to understand Device Tree
https://docs.zephyrproject.org/latest/guides/dts/howtos.html#devicetree-howtos

### Learn from the provided NRF and Zephyr samples!
https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/examples.html

### Working with NRF devices will have you working with regular AT Commands
https://infocenter.nordicsemi.com/index.jsp?topic=%2Fref_at_commands%2FREF%2Fat_commands%2Fmob_termination_ctrl_status%2Fmob_termination_ctrl_status.html

### Here is a full list and explanation of most AT Commands
https://infocenter.nordicsemi.com/pdf/nrf91_at_commands_v1.4.1.pdf

### Look at the various provided NRF libraries
https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/libraries.html

### Some User Guides
https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/user_guides.html

