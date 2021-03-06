Add "com.epson.escpos" in Supported External Accessory Protocol in your application info.plist

=========================================================================
          Epson ePOS SDK for iOS Version 2.3.0

          Copyright Seiko Epson Corporation 2015-2016 All rights reserved.
=========================================================================

1. About this software

The Epson ePOS SDK for iOS is an SDK aimed at development engineers who 
are developing iOS applications for printing on an EPSON TM printer and 
an EPSON TM Intelligent printer.
Applications are developed using the APIs provided by Epson ePOS SDK.
Epson ePOS SDK for Android for Android devices is also provided in 
Epson ePOS SDK.
For detailed information, please see Epson ePOS SDK for iOS User's Manual.

iOS Versions
  iOS 6.0 to 6.1.6
  iOS 7.0 to 7.1.2
  iOS 8.0 to 8.0.2
  iOS 8.2 to 8.4.1
  iOS 9.0 to 9.2.1

iOS Devices
  iPhone ( 4S / 5 / 5c / 5s / 6 / 6 Plus / 6s / 6s Plus )
  iPod touch ( 5th generation / 6th generation )
  iPad2 / iPad ( 3rd generation / 4th generation )
  iPad Pro ( 12.9-inch / 9.7-inch )
  iPad Air / iPad Air 2
  iPad mini / iPad mini 2 (iPad mini with Retina display) / iPad mini 3
   / iPad mini 4

Supported TM Printers
  EPSON TM-T20
  EPSON TM-T20II
  EPSON TM-T60
  EPSON TM-T70
  EPSON TM-T70II
  EPSON TM-T81II
  EPSON TM-T82
  EPSON TM-T82II
  EPSON TM-T88V
  EPSON TM-T88VI
  EPSON TM-T90II
  EPSON TM-P20
  EPSON TM-P60
  EPSON TM-P60II
  EPSON TM-P80
  EPSON TM-U220 series
  EPSON TM-U330 series
  EPSON TM-m10
  EPSON TM-m30

Supported TM Intelligent Printers
  EPSON TM-T20II-i
  EPSON TM-T70-i
  EPSON TM-T82II-i
  EPSON TM-T83II-i
  EPSON TM-T88V-i
  EPSON TM-U220-i
  EPSON TM-T70II-DT
  EPSON TM-T88V-DT
  EPSON TM-H6000IV-DT

Supported Network Printers
  EPSON TM-L90
  EPSON TM-T88IV
  EPSON TM-T90
  EPSON TM-H6000IV

Supported Interfaces
  TM Printer
    Wired LAN
    Wireless LAN
    Bluetooth
  TM Intelligent Printer
    Wired LAN
  Network Printers
    Wired LAN
    Wireless LAN

2. Supplied Files

- ePOS2.h
  Header file that includes class definitions and error value / device type 
  constant definitions.

- ePOSEasySelect.h
  Header file for selecting a printer easily

- libepos2.a
  Library for function execution 
    (armv7, armv7s, arm64, i386, x86_64 supported)

- libeposeasyselect.a
  Library for selecting a printer easily
    (armv7, armv7s, arm64, i386, x86_64 supported)

- ePOS_SDK_Sample_iOS.zip
  A sample program file

- EULA.en.txt
  Contains the SOFTWARE LICENSE AGREEMENT

- EULA.ja.txt
  Contains the SOFTWARE LICENSE AGREEMENT (The Japanese-language edition)

- ePOS_SDK_iOS_um_en_revx.pdf
  A user's manual

- ePOS_SDK_iOS_um_ja_revx.pdf
  A user's manual (The Japanese-language edition)

- ePOS_SDK_iOS_Migration_Guide_en_revx.pdf
  A migration guide

- ePOS_SDK_iOS_Migration_Guide_ja_revx.pdf
  A migration guide (The Japanese-language edition)

- README.en.txt
  This file

- README.ja.txt
  The Japanese-language edition of this file

3. Remarks

- For detailed information, please see Epson ePOS SDK for iOS User's Manual.

- Under TCP/IP connection at iOS9.x, set the default gateway address to the
  network router.

4. Restriction

- Discovery function of the following TM Intelligent printer doesn't support.

    TM-DT series (TM-DT software version 3.01 or earlier)
    TM-i  series

5. Version History

  Version 2.3.0
    - iOS 9.3.x was removed from support OS.
    - Added TM printer support
      - TM-T60
      - TM-m30 Korean model
    - Bug Fixed
      - Fixed disconnect API may not returned when the API is called.
        * This situation only happen with TM Intelligent Printers.

  Version 2.2.0
    - Added iOS versions support
      - iOS 9.3.2
    - Added iOS device support
      - iPad Pro ( 9.7-inch )
    - Added support for the following requirements of the App Store.
      - All apps submitted to the App Store must support IPv6-only networking.

  Version 2.1.0
    - Added TM printer support
      - TM-T88VI
    - Added iOS versions support
      - iOS 9.1 to 9.3.1
    - Added iOS device support
      - iPad Pro ( 12.9-inch )
    - Added Bitcode support
    - Added a Swift sample program(ePOS2_Printer_Swift)
    - Added a function getSdkVersion to retlieve SDK version in Epos2Log class
    - Improved TM-U220 functions.
      - Added double density of addImageAsync API in Printer class
      - Added second color of addTextStyle API in Printer class
      - Added addTextSize API in Printer class
      - Added addLogo API in Printer class
    - Bug Fixed
      - Fixed the rest of data is printed when OFFLINE condition happened
        while printing and then the OFFLINE condition is resolved.
      - Fixed printer status is "Connected" even though turn off printer
        while printing.
        * This situation only happen with TM-P20/TM-P60II/TM-m10/TM-m30/TM-T90II.
      - Fixed disconnection event may not occur when disconnect API is called.
      - Fixed the addFeedPosition API can not feed paper correctly.

  Version 2.0.0
    - New release