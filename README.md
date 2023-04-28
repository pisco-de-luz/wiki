# Welcome to the Pisco de Luz Social Project page!

<p>Imagine total darkness. Most of us can’t. We have lived in a world where power runs through everything - our devices, homes, and lives. However, for generations, residents of the Quilombola community in the region of Chapada dos Veadeiros had no access to electricity, condemning them to live in debilitating darkness every night. Living without power severely limits their productivity as well as social interactions.</p> 

<img src="https://github.com/pisco-de-luz/Social-Project/blob/3e8f8db801335711d6fdd490361ff9fb513b8117/images/Waking-with-oil-lamp2.gif" height="300"> <img src="https://github.com/pisco-de-luz/Social-Project/blob/6282648e4543a6c874d2b68f1cc8ab1c4c6eaf8e/images/lamparina-2.png" height="300">

<p>It also exposes them to life-threatening risks, such as animal attacks and hazardous fumes from diesel oil lamps. These lamps, which they use to illuminate their homes at night, have caused several housefires in which families have lost everything they had. This grim reality of the residents’ lives led to the creation of Pisco de Luz, with one purpose - to provide a little light in the darkness.</p>

<img src="https://github.com/pisco-de-luz/Social-Project/blob/3e8f8db801335711d6fdd490361ff9fb513b8117/images/triple-oil-lamp.gif" height="300"> <img src="https://github.com/pisco-de-luz/Social-Project/blob/6282648e4543a6c874d2b68f1cc8ab1c4c6eaf8e/images/lamparina-sebastiao.png" height="300">

<p>In July 2017, André had his first experience spending the night in the community,  using only diesel oil lamps. Diesel-burning smoke had already made the environment unbearable only two hours after sunset. It felt like being trapped in a garage with cars running. The worst is that his nostrils were full of soot the next day.</p>
<p>Shocked by the severity of the situation and determined to change it, André developed a low-cost solar-powered lighting system to provide sustainable and free light in people's homes. The first prototype was made on a protoboard, and once the circuit was stabilized, he implemented the first version on a universal board.</p>

<img src="https://github.com/pisco-de-luz/Social-Project/blob/7adf8b3d50c8d97672950180724e2c47a46d8786/images/First-kit-assembled.png" height="300">

<p>
Internally, the circuit consists of a buck converter that, when activated by the firmware, stabilizes the voltage of the solar panel at 5 volts. The internal ADC is used to measure the voltage from the solar panel both when the bulk converter is activated and when it is not.

The output of the bulk converter feeds the battery charger circuit, whose charging current is linearly controlled by the Arduino. An MPPT algorithm has been implemented to constantly analyze the relationship between the voltage delivered by the solar panel and the battery charging current.

The firmware also controls the charging and discharging of the battery, ensuring that the battery is not charged above 4.1 volts and disabling the boost converter and USB charger if the battery falls below 3.7 volts. Ensuring that the battery operates within this range significantly increases battery life. </p>

<img src="https://github.com/pisco-de-luz/Social-Project/blob/54976f91e0ab782d7e09ea7e6a8445cef78fc091/images/Electronic-Diagram.png" heights="300">

<p>Seven GPIOs are connected to the input of a Darlington array. This array is used to switch the LEDs in each room on and off independently. The 12V voltage is generated by the boost converter and is common to all rooms. 

Each room can have one or more switches and all of them have a small LED to make it easier to locate them when the room is completely dark. 

There is also a USB charger circuit that is only activated during the day when there is plenty of sun and the battery is fully charged. 

Finally, a serial port has been added to collect statistics and perform small calibrations when necessary.</p> 

<p> The solar kits consist of wires, LED lamps, a solar panel, and an intelligent controller using an Arduino Nano.</p>

<img src="https://github.com/pisco-de-luz/Social-Project/blob/3e8f8db801335711d6fdd490361ff9fb513b8117/images/Andre-assembling-first-kit.gif" height="300">

<p>The intelligent system monitors many variables, such as the usage hours of illumination, the amount of solar radiation, the minimum and maximum voltage of the battery, etc., delivered through the serial RS232 port.</p>

<img src="https://github.com/pisco-de-luz/Social-Project/blob/4311c8676f620b2a2a02716242866ea852a6016f/images/serial-stats.gif" height="300">

<p>In September 2017, after developing and assembling two kits, André returned to this community and installed them in two families. Since it was the first version of the kit, the installation process was quite demanding.</p>

<img src="https://github.com/pisco-de-luz/Social-Project/blob/db9510387bc06f73a6e9f5962beff37d9fcba867/images/One-of-the-First-Families-2017.png" height="300"> <img src="https://github.com/pisco-de-luz/Social-Project/blob/4311c8676f620b2a2a02716242866ea852a6016f/images/installing-solar-panel.gif" height="300"> 

<p>The cable system was composed of a four-color alarm cable connected using jelly crimp wire connectors. It worked well when André first tested this configuration in his at-home laboratory. However, when he went to install the kits in these first two houses, as they were very dark inside, it was pretty challenging to join them correctly.</p>


<img src="https://github.com/pisco-de-luz/Social-Project/blob/eef51eb9e24667499efe685995d8b2c24925a439/images/emenda-linear-p-tel-com-gel.jpg" height="300"> <img src="https://github.com/pisco-de-luz/Social-Project/blob/db9510387bc06f73a6e9f5962beff37d9fcba867/images/Installing-an-interruptor-inside.png" height="300">



Pisco de Luz assembles and installs solar-powered light kits in low-income communities with the help of volunteers.

# Bringing Dignity

We transform the lives of families who still live without access to electricity. 

# How?

We install a small solar panel on the roof, an intelligent circuit, a battery, various lights, and light switches throughout the homes.


https://user-images.githubusercontent.com/46757321/194868063-f188dee3-fed2-4298-a57a-0f44b3fbe241.mp4


<p aligh="center">


</p>

Same kitchen before and after Pisco de Luz's solar kit installation:
