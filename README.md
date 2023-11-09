# USB-Type-C-to-LoRa-Dongle-Software

USB Type-C to LoRa Dongle is a powerful and versatile LoRa device that lets you connect beyond boundaries. With its exceptional range and easy connectivity, it allows you to seamlessly communicate with devices up to 5 km away. LoRa Dongle is the perfect solution for anyone looking to establish long-range wireless communication in a variety of applications.

<!--
<img src = "https://github.com/sbcshop/Usb_To_LoRa_Dongle_Software/blob/main/Images/lora_usb.png"/>
-->

## Getting Started with USB to LoRa Dongle
* Device uses USB to TTL CH340 onboard, so make sure you have driver installed in your System to access LoRa Dongle via USB.
* Connect LoRa C dongle to system using usb cable and check your COM Port in device manager.
    
    <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/device_manager_comport_view.png" width="584" height="425">

    If you don't have CH340 driver installed in PC/laptop, then checkout [CH340 Driver Installation Manual Guide](https://github.com/sbcshop/NFC_Module/blob/main/documents/CH340%20Driver%20installation%20steps.pdf).

* To begin, select the jumpers indicated in the diagram below to configure the LoRa in transceiver mode:

  <img src = ""/>

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

### Operating Mode
 There are four operating modes, which are set by M1 and M0. Connecting jumper makes corresponding pin Logic 0 and open makes it Logic 1. 
 
 <img src = ""/>
 
 |Operating Mode | M1 | M0 |
 |---|---|---|
 |Normal Mode | 0 | 0 |
 |WOR Mode | 0 | 1 |
 |Configuration Mode | 1 | 0 |
 |Deep Sleep Mode | 1 | 1 |


## Resources
* [Schematic](https://github.com/sbcshop/Usb_To_LoRa_Dongle_Hardware/blob/main/Documents/sch%20USB%20LoRa%20Dongle.pdf)
* [Hardware Files](https://github.com/sbcshop/Usb_To_LoRa_Dongle_Hardware)


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

This is ***open source*** product. Kindly check LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=300">
</p>
