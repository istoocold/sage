Zdrasti! So I didn't remembers the exact dates so I will journalling accordint to lapse wise.
##  Week-1 
### [Lapse -1 ](https://lapse.hackclub.com/timelapse/STPKqnpzy198)

Intially this I was thinking of making a brick phone like design for game and as alarm , pager and AI voice assistant.Then I sketched the idea for finding proper fiting of future components.I researched for perfect MCU,  Mic and speaker amplifier.
I selected ESP-32 WROOM 38 pin.
I downloaded the symbol for KiCAD, it was messed up like wrong pin etc. 

### [Lapse-2](https://lapse.hackclub.com/timelapse/STPKqnpzy198) ~2.5 hrs

As I said in previous lapse I did changed the design. started with sketch place buttons etc , I tried made a design that can be hook in belt onon bags etc..It took around 10 mins.
Then we continue with  fixing pins arrangments and pin no.s. editing symbols. I took around 1.2 hours.Then I researched bout the display, I decided to go for 128x128 OLED display. Then added Con01x07 , then added corresponding symbols for Mic. For Mic I selected INMP441. and Then comes the Amplifier I choose very basic MAX98357 for 3.3 volts and a 5w speaker. Then Labeled and wired. Took around 1 hours and done!

### [Lapse-3](https://lapse.hackclub.com/timelapse/71GCBc5pgoB8) ~1.4 hrs 
Now started with power system and battery.
Now I dont want to use two battery for 5V power output so i use TPS61023 to boost the power to 5V
as capacitor will take in place for traded current.
Now comes the Charging part, previously I used a 7semi type C breakout board; I choose breakboard cz I found it easier to move and solder that a bare Type-C pin.
But with that I needed a charging IC with it for proper voltage regulation and chargin control.

Therefore, I used a TP4056 a complete breakout board with type-c pin and IC and charging lights.



Now started the navigation part so Initally used "switch" symbol but as it contail footprint of a push button direct on main board, I went for Conn_01x02 later I will prob add anothr thin PCB to add a push button on that board and connect it to two pad on main board as footprint; I found it convenient.Morover I added two more conn2 for pwr button and led and wire its resitor too.
Then Labeled and wired them accordingly.

### [Lapse-4](https://lapse.hackclub.com/timelapse/TPOkQQoscVtR) ~3 hrs
So I  started with reseaching rotary Enconder.
I went for EC-11 of 5 switch one for additional switch.I searched for their symbols . Then I searched around for voltage regulator to 3.3v  I selected MAX98357 , It was most easily available for me in market. Then head for it symbol, imported and wired all the component with respective GPIOs.

Now comes the part of assigning  footprint time. Now lets me give my plan so I don't really gonna solder evry componnet directly on board , it cause fitting n egronomics issue therefore I used pads to solder wire and then wire to the component.
I made custom pads of 1x3 to solder earlier. My mic need 7 pads but I didn't had one! so I edit and change and design a new footprint for it.
Similarly I assign footprint and started in pcb router.

I encountered a problem, many components have too many connection point, like 7 pads for display itself and they're just 1x3 mm n I sodler like horseshit. So opened the previous footprint again and expanded it to 2x6 mm and made like like 6 footprint from 2 to 7 pads.




While assigning footprints i forgot to assign footprint for MCU that is ESP 32- Wroom,  but When i sdoenladed that and imported all pins were messed up I rearragned the pins nos and serialised way .  IT took long cz later while routing I see I actally messed up with some numbering. And dis lapse compiles here.





### [Lapse-4](https://lapse.hackclub.com/timelapse/PQjQccj9YmX_) ~ 1.4 hrs
started with fixing the size for custom footprints it took long then I started placing the pads in pcb like placing gnd and corresponding GPIOs.Also I fucking did all naming wrongs like reference names cz this is my first hardware project.So I fixed them and simultaneously placing footprint and routing starting from there.



### [Lapse-5](https://lapse.hackclub.com/timelapse/weWDb_QQjbTG) ~ 1.7 hrs


So I mostly routed the components so Idk how to journal it, so for routing I used tracks of three width 0.1,0.2,0.5 mm. 0.5mm was for power lines. also  same for via, completed  my routing here.

### [Lapse-6](https://lapse.hackclub.com/timelapse/6RthYl_8jfdb) ~ 2.7 hrs
I started designing my case frome this lapse,