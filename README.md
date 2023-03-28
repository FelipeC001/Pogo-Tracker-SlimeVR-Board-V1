# Pogo-Tracker-SlimeVR-Board-V1
A repository for all the latest files on the Pogo Tracker and its charging base, 3D printable models, and PCB assembly guides.

## Description
A major challenge with pretty much all trackers today is requiring many USB charging cables to be able to charge up each of your trackers. This is especially cumbersome with 7 or even 10 trackers that each need their own cable to be charged at the same time. With this design all that is required to charge is one USB C cable connected to a dedicated charging base, and then you're able to stack each tracker on top of each other to charge. This allows for a less cluttered storage space for your trackers, and makes it even easier to just pick up and strap on them on to play.

This board completely open source and is meant to be fairly easy to put together without requiring a hand soldering tool or hand soldering experience. All that is needed is a soldering paste syringe, a set of thin tweezers, and a small hot plate to solder everything together at once. The PCB production files are readily available to be quickly manufactured through services like [JLCPCB](https://jlcpcb.com/) and [PCBWay](https://www.pcbway.com/), and component lists are available to be able to sourced through sites like [LCSC](https://www.lcsc.com/) and [Mouser Electronics](https://www.mouser.com/). The cases designed for the tracker and the charging base are meant to be easily 3D printed without supports , all that is needed is a machine with at least some tuning done to ensure there is no stringing or issues with bridging. 3D Printing services are also available through the PCB manufacturers previously mentioned.

If you'd like to purchase a set of premade boards or cases, or need help with anything, feel free to join the [Discord!](https://discord.gg/wSvvSv9sZJ) 

More board versions are planned around different IMU sensors, though they can also be modified by anyone for their own personal needs if they want.

## Features

* Stackable charging! Stack up to 10 trackers on a single charging base

* 5 hour battery life (500mAh battery)

* On/Off power button, no need for a switch!

* Built in diode protection and battery life sensor

* Expansion port for adding sensor extensions

* Low price (~$15 per tracker with recommended PCB and battery selection)

* No hand soldering or wire cutting needed, only a small hot plate to melt the solder paste

### Board Versions
V1 (Prototype)

### IMU's Currently Supported
BMI160

## How to source and order parts

 ### PCB
1. Find the zipped Gerber file of the board version you'd like, and upload it to one of the quote pages ([JLCPCB](https://cart.jlcpcb.com/quote?orderType=1&stencilLayer=2&stencilWidth=100&stencilLength=100&stencilCounts=5) or [PCBWay](https://www.pcbway.com/orderonline.aspx))

2. Select how many PCB's you'd like, minimum order is for 5 boards, with increments of 5 if you want more. 
    - First time customers usually to get discounts deals on the boards, especially with JLCPCB!

3. Select a board thickness of 1.6mm to ensure compatibility with the cases.

4. Select a board color.
    - Green has the quickest turn around time and is sometimes cheaper than the other colors!

5. Select a surface finish. Lead-free HASL is recommended for safety in handling, and is only around $1 extra for the total order on JLCPCB.

 #### Optional
 * You can order a stencil to be made along side the PCB, it's a metal sheet with cutouts for the metal pads on the board that can let you more easily put solder paste on the board. Stick with a sanding polish and no frame if you do order this for a small number of boards. Adds around $8 to the order price.

 * SMD Assembly is an option, but it is pricey and increases the production time significantly. It may also be unreliable, so be cautious!

 ### Components
You can hand select each component based off the schematic or BOM file, but if you wish to make the process automatic then I recommend sticking to LCSC with the BOM file.

 1. Take the BOM file and upload it to LCSC's [BOM tool.](https://www.lcsc.com/bom)
 
 2. On the drop-down menu of the first column, select LCSC Part Number. Then on the second column select Quantity. After that just hit next.
 
 3. Scroll down to ensure all parts are in stock. If it's all in stock then click on the top right to add all to cart, then check out and purchase.

 #### Out of stock items
 ***Do not try to substitute important components such as the battery management and power regulator with other similar parts, you risk damaging the board and battery if you don't know what you are doing!*** 
 
 If passive components (resistors, capacitors, etc) are out of stock, then it's possible to look for similar parts with the same values and footprint size in LCSC. For more specialized components like power and battery management IC's, look for the same model number on Mauser or any other part supplier site.

 ### Soldering
 You only need soldering paste, thin tweezers, and a little hot plate to assemble the board together. You can also use a hot air gun to solder, though be careful to not blow off components or damage parts due to excessive heat and stress.

 * ChipQuik NC191LTA10 is cheaply and readily available on amazon and is a good lead-free solder paste. Leaded versions are also available if you would prefer it.
 
 * ESD Tweezer sets are available on amazon, I recommend these to avoid accidentally damaging components due to static shock. They also come with different angles that make be easier to use.
 
 * A small hot plate for cooking with a pan from amazon should work if you pay close attention during the reflow process. There are also dedicated reflow hot plates available that are larger and more expensive, and even a cheap DIY kit for precision reflow cycle soldering with no risk. Link to the DIY kit can be found [here](https://github.com/AfterEarthLTD/Solder-Reflow-Plate), or may be available to purchase premade through the [Discord](https://discord.gg/wSvvSv9sZJ) if available!

 ### Cases
 Cases can be either printed yourself using PLA or PETG, or can be manufactured using the PCB services from above, although it tends to be very pricey even for the cheapest options. You can also buy cases if they are available in the [Discord](https://discord.gg/wSvvSv9sZJ) or commission someone to make them for you.

 ### Batteries
 The battery size for the official case is a 502248 3.7v Lipo battery. If they do not have JST connectors (2mm pitch) then you'll have to crimp them on or solder them yourself in the correct order.

 ***Make sure your battery has a built in protection board! The Lipo protection circuitry on the board is for charging only, make sure that discharge and over charge regulators are built into the battery you purchase.***


## How To Purchase premade
Stay tuned in the [Discord](https://discord.gg/wSvvSv9sZJ) channel for updates on availability!

## Assembly And Programming Guide

Assembly guide will be put up soon after the first prototypes arrive and are assembled using various techniques. Videos will also be made eventually for walking through each assembly step.

## Licensing
This project is backed by an MIT license, so feel free to share and modify the designs or even produce and sell them (just without a warranty or liability). All I ask is for credit if your project is based off off this design, and to support SlimeVR and its community!
