# autonomous robomaster
                Solution to an Autonomous RoboMaster
RoboMaster EP comes equipped with a power connection module (with IMU) and an intelligent controller unit, missing a controlling computer.
The solution is to mount a Raspberry Pi 3B+ via USB, that will control the RoboMaster running python programs on board.

![RobomasterEPwithRaspberryPI](https://github.com/stmarx/robomaster/assets/73398331/667a3e07-b3e3-4f4f-bb21-65f63b97cee6)


based on:
  - the RoboMaster EP robot hardware

![550d879b426848a0ecd0baf7f7917c5c](https://github.com/stmarx/robomaster/assets/73398331/ab9c6cca-032b-41c7-b444-c02192a62ab1)

              with RoboMaster power connection module with control IMU (Inertial measurement unit)
                        "     intelligent controller unit

  - Raspberry Pi 3B+

          - Broadcom BCM2837B0, Cortex-A53 (ARMv8) 64-bit SoC @ 1.4GHz.
          - 1GB LPDDR2 SDRAM.
          - 2.4GHz and 5GHz IEEE 802.11.b/g/n/ac wireless LAN, Bluetooth 4.2, BLE.
          - Gigabit Ethernet over USB 2.0 (maximum throughput 300 Mbps)
          - Extended 40-pin GPIO header.
    ![RaspberryPi3B+5ZollTouchscreen](https://github.com/stmarx/robomaster/assets/73398331/fed2b1cc-f7c3-4f94-b285-e52dac94c307)

                with "Buster" Debian + Python 3.7 system
                     3,5" Touchscreen  
                     running Debian Desktop

  - USB connections

![image](https://github.com/stmarx/robomaster/assets/73398331/6b3fa041-44ba-41d0-901d-57b07908224c)
      Raspberry Pi 3B+ _________________________________ power connection module ________________ intelligent controller unit

    - 5V to RM power connection module (RM power just sufficient for Raspberry Pi 3B+)
    - USB network to RM intelligent controller unit
      activated by start of RNDIS on Debian Linux
          run a Linux .sh with the following commands:
          $ ifconfig
          $ sudo dhclient -v usb0

  - the RoboMaster SDK as Python packackage "robomaster" on the Raspberry Pi

    install neccessary extensions and packages before you install "robomaster 0.1.1.62" under Python 3.7:
    Package             Version
    ------------------- --------
    pip                 23.3.1
    colorzero           2.0
    Cython              3.0.5
    future              0.18.2
    futures             3.0.5
    gast                0.2.2
    gpiozero            2.0
    h5py                3.8.0
    imageio             2.31.2
    Keras-Applications  1.0.8
    Keras-Preprocessing 1.1.1
    mock                3.0.5
    MyQR                2.3.1
    netaddr             0.8.0
    netifaces           0.10.0
    numpy               1.19.4
    opencv-python       4.8.1.78
    pbr                 6.0.0
    Pillow              9.5.0
    pkg_resources       0.0.0
    protobuf            4.24.4
    pybind11            2.11.1
    pyserial            3.5
    setuptools          49.6.0
    six                 1.16.0
    testresources       2.0.1
    wheel               0.41.3

  - Python editor connected to the RM Python 3.7

optional:

  - LEGO Technic extenstions
        - 4 LEGO Technic Beam 15
        - 2 LEGO Technic Beam Frame 5
