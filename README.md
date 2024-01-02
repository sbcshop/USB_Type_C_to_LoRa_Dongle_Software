# USB Type C to LoRa Dongle Software

USB to LoRa Dongle is a powerful and versatile LoRa device that lets you connect beyond boundaries. With its exceptional range and easy connectivity, it allows you to seamlessly communicate with devices up to 5 km away. LoRa Dongle is the perfect solution for anyone looking to establish long-range wireless communication in a variety of applications.

<!--
<img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/lora_usb.png"/>
-->

## Getting Started with USB to LoRa Dongle
* Device uses USB to TTL CH340 onboard, so make sure you have driver installed in your System to access LoRa Dongle via USB.
* Connect LoRa C dongle to system using usb cable and check your COM Port in device manager.
    
    <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/device_manager_comport_view.png" width="584" height="425">

    If you don't have CH340 driver installed in PC/laptop, then checkout [CH340 Driver Installation Manual Guide](https://github.com/sbcshop/NFC_Module/blob/main/documents/CH340%20Driver%20installation%20steps.pdf).

* To begin, make sure to have jumpers as indicated in the diagram below to set the LoRa in transceiver mode:

  <img src = "https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/blob/main/images/normal_mode.png"/>

* You can download the XCTU from link : [Download XCTU](https://hub.digi.com/support/products/xctu/)
   
* To transfer data, you can use XCTU or Tera Term for Windows, as well as other related software. XCTU is the most effective and user-friendly. 
  Follow the steps suggested below:

  <img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/img4.png"/>
  <img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/img5.png"/>
  <img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/img6.png"/>
  <img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/img7.png"/>
  <img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/img10.png"/>
  <img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/img11.png"/>

* It receives data from other LoRa Dongles, as shown in the image below.
  
  <img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/img12.png"/>
  <img src = "https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/blob/main/images/usb_c.png "/>

  Here

  **RX --> Data send by LoRa to computer via USB**
  
  **TX --> Data receive by LoRa to computer via USB**
  
### Operating Mode
 There are four operating modes, which are set by M1 and M0. Connecting the jumper makes the corresponding pin Logic 0 and opening makes it Logic 1. 
 
 <img src = "https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/blob/main/images/Mode_selection.jpg" width="502" height="320"/>
 
 |Operating Mode | M1 | M0 |
 |---|---|---|
 |Normal Mode | 0 | 0 |
 |WOR Mode | 0 | 1 |
 |Configuration Mode | 1 | 0 |
 |Deep Sleep Mode | 1 | 1 |

 For example, 
* Normal Mode 

  <img src = "https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/blob/main/images/normal_mode.png"/>

 * Config Mode

   <img src = "https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/blob/main/images/config_mode.png"/>

### LoRa Dongle As Breakout
UART serial pins of LoRa are breakout in the header and screw terminal form. So, this device can be used as a breakout to connect with any microcontroller or MCU. 

<img src = "https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/blob/main/images/LoRa_uart_pins.png" width="445" height="262"/>

How to interface LoRa with Microcontroller
 |Microcontroller | LoRa Device |
 |---|---|
 |5V | 5V |
 |TX | RX |
 |RX | TX |
 |GND | GND |


### Lora GUI For Configuration (run with the help of GUI)

 Follow the steps to configure the Lora module:-

 #### Step 1: Set up Lora in configuration mode, short M0, and open M1 as shown in the figure. 
 
  <img src= "https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/blob/main/images/config_mode.png" />
 
#### Step 2: Connect LoRa dongle to PC/laptop USB. Download and open [lora GUI application](https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Software/tree/main/GUI%20For%20Window) for Windows available in GitHub here
 <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img_1.png" />
 
#### Step 4: Connect the LoRa dongle to the system and Open Device Manager to know the correct COM port
  <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img_7.png" />
 
#### Step 5: Write the proper COM Port in the GUI and provide the baud rate, then press the connect button
  <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img_8.png" />
  <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img_9.png" />

#### Step 6: Press the red button to see the device configuration that Lora already has
  <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img__10.png" />
 
#### Step 7: Write the values which you need to configure, for eg: I configure channel and baud rate, after that press the write button
  <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img_13.png" />

 How to Set Corresponding Frequency:
 
    -> For changing frequency using Software for 868MHz & 915MHz LoRa module:

    Frequency = 850.125MHz + CH*1MHz
    
    0-83 total of 84 Channel available
    
    So, when 5 selected Frequency = 850.125MHz + 5*1MHz Frequency = 855.125MHz
    
    -> For Changing Frequency using Software for 433MHz LoRa Module: Frequency = 410.125MHz + CH*1MHz
    
    0-83 total of 84 Channel available
    
    So, when 5 selected Frequency = 410.125MHz + 5*1MHz Frequency = 415.125MHz
    
#### Step 8: Restart the GUI, set baudrate and port, then connect and press the read button 
  <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img_14.png" />
  <img src= "https://github.com/sbcshop/Lora-HAT-for-Raspberry-Pi/blob/main/images/img_15.png" />


## Resources
* [USB Type C to LoRa Dongle Schematic](https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Hardware/blob/main/Design%20Data/SCH%20LoRa%20C.pdf)
* [USB Type C to LoRa Dongle Hardware Files](https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Hardware)
* [USB Type C to LoRa Dongle Step File](https://github.com/sbcshop/USB_Type_C_to_LoRa_Dongle_Hardware/blob/main/Mechanical%20Data/Step_LoRa_C.step)


## Related Products
  * [LoRa HAT For Raspberry Pi](https://shop.sb-components.co.uk/products/lora-hat-433mhz-868mhz) 
  
     ![LoRa HAT For Raspberry Pi](https://cdn.shopify.com/s/files/1/1217/2104/products/lora.jpg?v=1670911119&width=300)
    
  * [USB to LoRa Dongle](https://shop.sb-components.co.uk/products/lo-fi?variant=41026475753555) 
   
     ![USB to LoRa Dongle](https://shop.sb-components.co.uk/cdn/shop/products/05_2.png?v=1678712489&width=300)   

  * [GatePi](https://shop.sb-components.co.uk/products/gatepi?variant=39756684066899) 
   
     ![GatePi](https://shop.sb-components.co.uk/cdn/shop/products/GatePi-4channelRelayBoardwithLoRaModulebasedonRP2040.jpg?v=1647335212&width=300) 

  * [RangePi](https://shop.sb-components.co.uk/products/range-pi?variant=39744084705363) 
   
     ![RangePi](https://shop.sb-components.co.uk/cdn/shop/products/1_54b19023-5d19-4f55-acea-af894f2d00c6.png?v=1646815358&width=300)

  * [Pico LoRa Expansion](https://shop.sb-components.co.uk/products/pico-lora-expansion-868mhz?_pos=5&_sid=8faf72598&_ss=r) 
   
     ![Pico LoRa Expansion](https://shop.sb-components.co.uk/cdn/shop/products/pico-expansioonpng_1_2525bf59-655f-421d-ac62-71e706c96060.png?v=1647321524&width=300)

 
## Product License

This is ***open source*** product. Kindly check the LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=300">
</p>
