# autonomous robomaster
                Solution to an Autonomous RoboMaster
RoboMaster EP comes with a power connection module (with IMU) and an intelligent controller unit, missing a computer.
The solution is to mount a Raspberry Pi 3B+ that can control the RoboMaster running python programs on board.

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
      Raspberry Pi 3B+ ____________________________________________ power connection module __________________ intelligent controller unit
