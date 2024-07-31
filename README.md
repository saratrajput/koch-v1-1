# Alexander Koch Arm V1.1

This folder contains the instructions to assemble a slightly modified version of the [Alexander Koch Arms](https://github.com/AlexanderKoch-Koch/low_cost_robot). 

For the curious reader, here are the most significant changes made:
1. Made small improvements to the hardware model including but not limited to: fixed screw interferences, cleaned up extraneous material, standardized hole sizes, removed screws fastening into plastic, added board platform to leader robot.
2. Added a platform for the leader arm. While not strictly necessary, this platform allows the follower arm to pick objects off the ground which it could not do in the previous configuration.
3. Removed the need for a soldering iron to assemble and for manually adjusting the voltage convertor, by replacing the DC convertor.
4. Added SolidWorks models to make it easier for the community to contribute.
5. Added a wiring diagram.
6. Added assembly video for leader and follower arm with SW animations.

## Assembly Instructions

### Sourcing Parts
Order the off the shelf parts for the leader and follower arm using the links below. Note prices and items may vary slightly depending on geographic location.

#### Leader Arm

| Part | Amount | Unit Cost (US) | Buy US | Unit Cost (EU) | Buy EU | Unit Cost (UK) | Buy UK |
|---|---|---|---|---|---|---|---|
| Dynamixel XL330-M077-T | 6 | $24 | [Robotis](https://www.robotis.us/dynamixel-xl330-m077-t) | 40€ | [MyBotShop](https://www.mybotshop.de/DYNAMIXEL-XL330-M077-T)-[GenRobots](https://www.generationrobots.com/en/403818-dynamixel-xl330-m077-t-servo-motor.html) | £27 | [RoboSavvy](https://robosavvy.co.uk/robotis-dynamixel-xl330-m077-t.html) |
| XL330 Frame and Idler Wheel 4pcs set<sup>[1](#myfootnote1)</sup> | 1 | $10 | [Robotis](https://www.robotis.us/fpx330-h101-4pcs-set) | 12€ | [GenRobots](https://www.generationrobots.com/en/403860-FPX330-H101-hinge-frame-and-idler-set-dynamixel-xl330.html) | £10 |  [RoboSavvy](https://robosavvy.co.uk/fpx330-h101-4pcs-set.html) |
| Waveshare Serial Bus Servo Driver Board | 1 | $10 | [Amazon](https://a.co/d/7C3RUYU) | 6€ | [GenRobots](https://eckstein-shop.de/WaveShare-Serial-Bus-Servo-Driver-Board-for-ST-SC-Serial-Bus-Servos-EN) | £8 | [Amazon](https://www.amazon.com/Waveshare-Integrates-Control-Circuit-Supports/dp/B0CTMM4LWK/) |
| 5V Power Supply | 1 | $6 | [Amazon](https://a.co/d/5u90NVp) | 9€ | [Amazon](https://www.amazon.fr/LEYF-Alimentation-Universelle-Adaptateur-Enfichable/dp/B09NGVWBSY) | £4 | [Amazon](https://a.co/d/5u90NVp)|
| Jumper Wires 3*40 pcs set (M-M, M-F, F-F) | 1 | $7 | [Amazon](https://a.co/d/hQfk2cb) | 9€ | [Amazon](https://www.amazon.fr/AZDelivery-Jumper-Cavalier-C%C3%A2ble-Arduino/dp/B074P726ZR) | £5 | [Amazon](https://a.co/d/hQfk2cb)|
| Table Clamp | 1 | $6 | [Amazon](https://a.co/d/4KEiYdV) | n/a | n/a | £5 | [Amazon](https://a.co/d/4KEiYdV) |
| Table Clamp 4pcs set<sup>[2](#myfootnote2)</sup> | 1 | n/a | n/a | 14€ | [Amazon](https://www.amazon.fr/CAUTIOUS-Serre-Joint-R%C3%A9glable-Serre-Joints/dp/B0CJMB3SKH) | n/a | n/a |
| 1.5mm Star/Cruciform Screwdriver 2pcs set | 1 | n/a | n/a | 7€ | [Amazon](https://www.amazon.fr/sourcing-map-Cruciforme-%C3%89lectroniques-R%C3%A9paration/dp/B0BQ69J2QF) | n/a | n/a |
| 1.5mm Star/Cruciform Screwdriver included in set | 1 | $6 | [Amazon](https://www.amazon.com/Choice-9-Piece-Precision-Screwdriver-Phillips/dp/B0747DYJJR) | n/a | n/a | £5 | [Amazon](https://www.amazon.com/Choice-9-Piece-Precision-Screwdriver-Phillips/dp/B0747DYJJR)
| Total | | $189 | | 297€ | | £199 | |

#### Follower Arm

| Part | Amount | Unit Cost (US) | Buy US | Unit Cost (EU) | Buy EU | Unit Cost (UK) | Buy UK |
|---|---|---|---|---|---|---|---|
| Dynamixel XL430-W250-T |  2 | $50 | [Robotis](https://www.robotis.us/dynamixel-xl430-w250-t) | 57-61€ | [MyBotShop](https://www.mybotshop.de/DYNAMIXEL-XL430-W250-T)-[GenRobots](https://www.generationrobots.com/en/402823-dynamixel-xl430-w250-t-servomotor.html) | £47 | [RoboSavvy](https://robosavvy.co.uk/dynamixel-xl430-w250-t.html)
| Dynamixel XL330-M288-T |  4 | $24  | [Robotis](https://www.robotis.us/dynamixel-xl330-m288-t) | 40-46€ | [MyBotShop](https://www.mybotshop.de/DYNAMIXEL-XL330-M288-T)-[GenRobots](https://www.generationrobots.com/en/403817-dynamixel-xl330-m288-t-servo-motor.html) | £27 | [RoboSavvy](https://robosavvy.co.uk/robotis-dynamixel-xl330-m288-t.html) |
| XL330 Frame and Idler Wheel 4pcs set<sup>[1](#myfootnote1)</sup> |  1 | $10 | [Robotis](https://www.robotis.us/fpx330-h101-4pcs-set) | 12€ | [GenRobots](https://www.generationrobots.com/en/403860-FPX330-H101-hinge-frame-and-idler-set-dynamixel-xl330.html) | £10 |  [RoboSavvy](https://robosavvy.co.uk/fpx330-h101-4pcs-set.html) |
| XL430 Idler Wheel set | 1 | $7 | [Robotis](https://www.robotis.us/hn11-i101-set) | 9€ | [GenRobots](https://www.generationrobots.com/en/403206-hn11-i101-horn-set.html) | £7 | [Robosavvy](https://robosavvy.co.uk/hn11-i101-set.html)|
| Waveshare Serial Bus Servo Driver Board | 1 | $10 | [Amazon](https://a.co/d/7C3RUYU) | 6€ | [Eckstein](https://eckstein-shop.de/WaveShare-Serial-Bus-Servo-Driver-Board-for-ST-SC-Serial-Bus-Servos-EN) | £8 | [Amazon](https://www.amazon.com/Waveshare-Integrates-Control-Circuit-Supports/dp/B0CTMM4LWK/)|
| Voltage Reducer | 1 | $14 | [Amazon](https://www.amazon.com/EPLZON-Converter-5V-5-3V-Transformer-Regulator/dp/B09R4DBZJK) | 7€ | [Amazon](https://www.amazon.fr/ICQUANZX-Converter-Transformer-Voltage-Regulator/dp/B07RGB2HB6) | £11 | [Amazon](https://www.amazon.com/EPLZON-Converter-5V-5-3V-Transformer-Regulator/dp/B09R4DBZJK) |
| 12V Power Supply | 1 | $12 | [Amazon](https://a.co/d/40o8uMN) | 15-36€ | [Amazon](https://www.amazon.fr/LEDMO-Alimentation-Adaptateur-Transformateurs-Chargeur/dp/B07PGLXK4X)-[GenRobots](https://www.generationrobots.com/en/400866-smps-charger-for-bioloid-and-dynamixel-robotis.html) | £9 | [Amazon](https://a.co/d/40o8uMN) |
| Jumper Wires 3*40 pcs set (M-M, M-F, F-F) | 1 | $7 | [Amazon](https://a.co/d/hQfk2cb) | 9€ | [Amazon](https://www.amazon.fr/AZDelivery-Jumper-Cavalier-C%C3%A2ble-Arduino/dp/B074P726ZR) | £5 | [Amazon](https://a.co/d/hQfk2cb) |
| Table Clamp | 1 | $6 | [Amazon](https://a.co/d/4KEiYdV) | n/a | n/a | £5 | [Amazon](https://a.co/d/4KEiYdV) |
| Table Clamp 4pcs set<sup>[3](#myfootnote3)</sup> | 1 | n/a | n/a | 14€ | [Amazon](https://www.amazon.fr/CAUTIOUS-Serre-Joint-R%C3%A9glable-Serre-Joints/dp/B0CJMB3SKH) | n/a | n/a |
| 1.5mm Star/Cruciform Screwdriver 2pcs set<sup>[4](#myfootnote4)</sup> | 1 | n/a | n/a | 7€ | [Amazon](https://www.amazon.fr/sourcing-map-Cruciforme-%C3%89lectroniques-R%C3%A9paration/dp/B0BQ69J2QF) | n/a | n/a |
| 1.5mm Star/Cruciform Screwdriver included in set<sup>[4](#myfootnote4)</sup> | 1 | $6 | [Amazon](https://www.amazon.com/Choice-9-Piece-Precision-Screwdriver-Phillips/dp/B0747DYJJR) | n/a | n/a | £5 | [Amazon](https://www.amazon.com/Choice-9-Piece-Precision-Screwdriver-Phillips/dp/B0747DYJJR) |
| USB C-A or C-C 2pcs set (1 pc needed) | 1 | $9 | [Amazon](https://www.amazon.com/Charging-etguuds-Charger-Braided-Compatible/dp/B0B8NWLLW2/) | 7€ | [Amazon](https://www.amazon.fr/-/en/dp/B0CKPDZ3SK/) | £7 | [Amazon](https://www.amazon.com/Charging-etguuds-Charger-Braided-Compatible/dp/B0B8NWLLW2/)|
| Total | | $277 | | 360€ | | £269 | |

### Printing the Parts
A variety of 3D printers are acceptable to print the parts necessary of the follower and leader arm. Follow the steps below to ensure a good print.

1. Choose a printer: When choosing a printer there are a variety of factors to consider. Below are the suggested printed settings, although using a printer outside these parameters may likely work as well.
   1. Precision: 0.2mm minimum height layer<sup>[5](#myfootnote5)</sup>
   2. Material: PLA, ABS, PETG or other reasonably strong plastics.
   3. Nozzle Diameter: 0.4mm maximum nozzle diameter
   4. Infill Density: ~30% <sup>[6](#myfootnote6)</sup>
   5. Sample Printers: [Prusa Mini+](https://www.prusa3d.com/product/original-prusa-mini-semi-assembled-3d-printer-4/), [Bambu P1](https://us.store.bambulab.com/collections/p1-series/products/p1p), [Ender3](https://www.amazon.com/Comgrow-Creality-Ender-Aluminum-220x220x250mm/dp/B07BR3F9N6/), etc.  
2. Set up the printer
   1. Materials:<sup>[7](#myfootnote7)</sup>
      1. [Standard Glue Stick](https://www.amazon.com/Amazon-Basics-Washable-School-Sticks/dp/B0CRCWCGNW/)
      2. [Putty Knife](https://www.amazon.com/Warner-ProGrip-Putty-Knife-90133/dp/B000I1VEK6/)
   2. Setup and Takedown
      1. Ensure that the printer is calibrated and the bed level is correctly set using the printer specific instructions.
      2. Clean the print bed, making sure it is free from dust, or grease. If cleaning the bed using water, or other liquid, dry the bed.
      3. Use a standard glue stick and apply a thin, even layer of glue across the print area of the bed. Avoid clumping or uneven application.
      4. Load the printer filament using printer specific instructions.
      5. Ensure the printer settings match the ones suggested above (most printers have multiple settings so choose the ones that most closely match).
      6. Choose the file(s) to print as found in the harware folder.
3. Print one of each of parts found in `hardware/leader/STL` and `hardware/follower/STL`, which are listed below.
   1. Leader:
      1. Leader_Base
      2. Leader_Elbow_To_Wrist
      3. Leader_Elbow_To_Wrist_Extension
      4. Leader_Gripper_Handle
      5. Leader_Gripper_Trigger
      6. Leader_Shoulder_To_Elbow
      7. Leader_Platform<sup>[8](#myfootnote8)</sup>
      8. Robotis_FPX330_S101<sup>[9](#myfootnote9)</sup>
   2. Follower:
      1. Follower_Base
      2. Follower_Elbow_To_Wrist
      3. Follower_Elbow_To_Wrist_Extension
      4. Follower_Gripper_Moving_Part
      5. Follower_Gripper_Static_Part
      6. Follower_Shoulder_Rotation
      7. Follower_Shoulder_To_Elbow
4. Take Down
   1. After the print is done, use the putty knife to scrape the the parts off the print bed.
   2. Remove any support material from parts.
   3. Reapply the glue stick before starting the next print.

### Assembling the Parts
Construct the leader and follower arms using the Assembly Video linked below.
Video of the Assembly: [Youtube](https://youtu.be/LilDX6zS6OY?si=ZD-oKlPLFzF46wV9) #TODO: Update with the new Youtube Video later.

### Configure
While this robot can be programmed in a variety of manners, it is suggested to use with [LeRobot](https://github.com/huggingface/lerobot/blob/133d184a544443b44095c83156dbf8d212ccfaf6/examples/7_get_started_with_real_robot.md). #TODO: Add link to exact tutorial.


### Footnotes
<a name="myfootnote1">1</a>: You will only use three idler wheels that come in this four piece set.\
<a name="myfootnote2">2</a>: You will only need one clamp in this 4 piece set.\
<a name="myfootnote3">3</a>: If you bought the 4 piece clamp set for the leader arm, you will not need to buy it again here, as only one clamp is necessary of the follower arm, and one for the leader arm.\
<a name="myfootnote4">4</a>: If you bought the screwdriver set for the leader arm, you will not need to buy it again here as the same screwdriver is used for the follower and leader arm.\
<a name="myfootnote5">5</a>: This precision is based on the fact the through holes for M2 fasteners are 2.4mm in diameter while the nominal diameter of a M2 fastener is 2mm. In a worst case scenario, this allows +/- 0.2mm while still allowing for screw alignment. However, if you are only capable of printing with a larger layer height, you will likely be fine, just ensure the screw holes align as expected.\
<a name="myfootnote6">6</a>: It is quite possible a lower density infill could be used, however, erring on the side of caution, I used 37% to ensure strong parts.  \
<a name="myfootnote7">7</a>: You do not need to buy these exact parts, but a glue stick and putty knife are almost always necessary for a good 3D print. The glue prevents parts from sticking to the print bed, and the putty knife helps scrape parts from the print bed. However, feel free to check with your specific printer instructions for if these parts are necessary. \
<a name="myfootnote8">8</a>: This is not strictly necessary to print but does allow the follower arm to reach the ground which is is otherwise unable to do in the current setup.\
<a name="myfootnote9">9</a>: You can either buy the Robotis [FPX330-S101](https://www.robotis.us/fpx330-s101-4pcs-set/), or 3D print it, but it is cheaper to print.