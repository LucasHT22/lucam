# June 30: Night session with footprints

Assigned footprints and imported all to PCB! now the pain of routing...

![](/assets/jun30_n1.png)

Time spent on this: 1 hours

# June 30: Finish Sheets

I've worked on my compute & sensor session

1. compute sch
 - connected pins of DF40 based on CM4 datasheet
    - j1 & j2
    - defined cm4_3v3_out and cm4_1v8_out
    - net labels net labels
    - i2c
    - spi
    - sd card
    - uart
    - usb
    - no connect

![](/assets/jun30.png)

2. sensor sch
 - connector fpc-22 pin added and footprint associated
 - net labels
 - pull ups
 - decoupling

![](/assets/jun30_0.png)

3. display sch
 - pin header
 - followed ILI9341 datasheet for pins
 - mosfet to control display backlight

![](/assets/jun30_1.png)

4. storage_ui sch
 - sd card pins with card detect pin
 - pull up resistors and capacitor decoupling
 - flash qspi
 - updates to compute sch, net labels
 - shutter button
 - status led: power and process
 - debug header uart

![](/assets/jun30_2.png)
![](/assets/jun30_3.png)

Time spent on this: 5 hours

# June 29: Night Session

I took this time after dinner to:
 - config symbol and footprints libs as cherrycam
 - added df40 from snapeda
 - choose footprint for fpc 22 pin
 - hierarchy sheets created
 - done power schematic: decoupling capacitors, polyfuse, ldos etc

![](/assets/Captura%20de%20tela%202026-06-29%20222719.png)

There's 3 ERC error raising that I have no idea why.

Time spent this session: 4 hours

# June 29: General planning

That's not my first attempt in making a camera, so I decided to start by creating 1 documents:
1. [Requirements](/requirements.md) - Made with the idea to not lose focus 

Next doc to be made is:
2. [Step by Step](/step-by-step.md) - so I can follow a guide

Also started KiCad project in: [cherrycam folder](/cherrycam/)

And gathered a few documents in [datasheets folder](/datasheets/)

My main problem is that I need to fit everything in a 7x5cm board so it's a proper digicam, but I'll start with a 7x10cm PCB so I can try different things on this V1, more space to work.

Time spent this session: 2 hours