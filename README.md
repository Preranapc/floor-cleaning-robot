#Team Members
-Prerana P Chavadi
-Namala Chandra Veditha



Step 1: Parts and Tools
The following parts and tools are required for building this project:

Parts:

-2x 100rpm Geared motors
-2x Wheels for motors
-2x 75rpm Plastic geared motors w/ wheels
-1x Arduino UNO
-1x HC-05/06 bluetooth module
-1x L293D motor driver board
-1x Standard servo motor (180 degree rotation)
-1x 12V Sealed lead acid rechargeable battery
-1x 12V Water pump
-2x TIP31C/TIP122 NPN power transistors
-2x Old CDs
-A paint roller w/ shaft
-Wiping cloth/ napkin/ old rags
-A needle and thread
-Vinyl tubing
-Rainbow wire
-Male-male/ female-female/ male-female jumper wires
-Male/female headers
-Perforated board
-Nuts and Screws
-Plywood base
-Paint roller w/ shaft
-A 600ml plastic bottle


Tools:

-Soldering iron w/ solder
-Hot glue gun w/ glue sticks
-Drill
-Rotatory tool
-Pliers
-Wire cutter/stripper
-Paper cutter
-Tape
-Safety equipment while working (Important!)


Total cost of the parts: $30 approx. (2000 rupees)

Step 2: Get the Base Ready
Get the Base Ready
Get the Base Ready
Get the Base Ready
Get the Base Ready
View 3 more
The first step is to prepare the base on which the parts will be placed. For this, first get a piece of plywood cut, measuring 12x9 inches. The base wasn't looking great at all, so to make it look a bit attractive, I painted it in white and orange stripes with black at the borders with acrylic paints.

After this, drill two holes each at the back for both the motor clamps. Make proper measurements such that both should be parallel to each other. Fix them in place using some screws then attach the motors to the clamps.

Step 3: Make the Floor Moppers and Attach Them to the Base
Make the Floor Moppers and Attach Them to the Base
Make the Floor Moppers and Attach Them to the Base
Make the Floor Moppers and Attach Them to the Base
Make the Floor Moppers and Attach Them to the Base
View 15 more
I found this idea on one of the YouTube videos (click here). To make cheap DIY circular floor moppers, you can use old compact disks along with a piece of cloth.

First mark a circle on the cloth which should be bigger than the CD. Cut it using a pair of scissors.

Take a needle and thread and start sewing and making folds to the cloth in such a way that it surrounds the entire CD. (something I am very bad at)

Refer to the images above or have a look at this video, or maybe this one.

After you're done with all the folds, make 2-3 knots at the end and cut the left over thread.

Repeat the same for the second CD.

Attach wheels to both the plastic geared motors. Hot glue the wheels to the CDs.

The moppers have to be placed in the front. Hot glue the motors in such a way that the cloth stays away from each other and the motors are at an equal distance from the sides. Make sure the cloth properly touches the floor

Step 4: The Water Supply Mechanism
The Water Supply Mechanism
The Water Supply Mechanism
The Water Supply Mechanism
View 12 more
This consists of a 12V water pump which carries the water from the reservoir and spills it near the mops on the floor. First mark, drill and fix your pump in place.

Take a 600ml empty plastic bottle and cut it into half using a paper cutter. Use the lower half and place it on the robot base using some hot glue.

Take two pieces of rubber tubing. One will be connected to the inlet of pump to take water from the reservoir from the pump and the second one will be used to take water from the pump to the floor. Adding straws to the outlet will be done later.

The pump can be switched on/off via your smartphone just like other controls.

Step 5: Roller Mechanism
Roller Mechanism
Roller Mechanism
Roller Mechanism
View 14 more
The purpose of roller here is to stick small dust particles to itself. It will not be needed everytime the robot is moving so I decided to make a simple mechanism which can lift it up or down via a servo motor.

First you need to drill a hole on the servo attachment. Drill another hole of almost same size on the roller handle as well. Use a screw to tighten the attachment and the roller.

The motor will have to be placed at a height so the roller touches the floor and can be lifted easily. Use two 7x2.5 centimetres wooden pieces and hot glue the servo to their top.

Step 6: Solder the Circuits
Solder the Circuits
Solder the Circuits
Solder the Circuits
View 6 more
For the mop geared motors and the water pump to be controlled via arduino, there has to be an external circuit as both of them need 12V to run but arduino can only provide a 5V output. I used TIP122 NPN power transistors and soldered them on to a piece of perfboard. The circuit is simple and is provided above.

Also, I soldered some male and female headers to make +5V and Gnd power rails as these pins are limited on the arduino and we need plenty of them for each component to be connected. Follow the pictures above and solder two rails, one for each +5V and Gnd.

Step 7: Connections
Connections
Connections
Connections
View 24 more
Now this is always the typical part. You have to be accurate. For making it a bit easier, I always use jumper wires which can be swapped or removed any time.

Before that, drill some holes and fix your arduino in place using some screws.

Start by connecting the geared motors to the driver board. Solder some wire to the motor terminals and then connect them to the screw terminals of the driver circuit. The rest of the pins have to be connecting as per the following:

Signal 1 ---- D6 on Arduino
Signal 2 ---- D9 on Arduino
Signal 3 ---- D10 on Arduino
Signal 4 ---- D11 on Arduino
+5V ---- +5V on Arduino
Gnd ---- Gnd on Arduino
+12V (motors will move at this voltage) ---- to be connected to battery later
Next comes the bluetooth module. Connections are:

Vcc ---- +5V on Arduino
Gnd ---- Gnd on Arduino
Rx ---- Tx on Arduino
Tx ---- Rx on Arduino
Add a voltage divider to signal pins if you're afraid that the signal pins on arduino might burn.

The two mop motors have to be connected in parallel such that the left one runs anticlockwise and the right one turns clockwise when seen from the front. Use heat shrink tubes to keep the connections safe. Solder the motor wires to the transistor circuit as per the schematic given above. Similarly connect the water pump wires as well.

We will be supplying the 12V from the battery directly to the transistor circuit and then this 12V will go to the Vcc of arduino and the motor driver circuit.

Connect the base of transistor two, controlling the mops to D5 on arduino and transistor one, controlling the pump to D4 on arduino. The common ground wire from all the motors has to be connected to the Gnd on arduino.

What remains now is the servo motor. The connections are:

Vcc ---- +5V on Arduino
Gnd ---- Gnd on Arduino
Signal ---- D3 on Arduino
You can always have a look at the schematic.

Step 8: Finishing
Finishing
Finishing
Finishing
View 11 more
Keep all the circuit boards, wires, tubings in place with hot glue. It should look neat, the wires shouldn't entangle and the connections shouldn't break, which can be irritating.

Next, take two straws and cut them about 7cm in length. Crush and squeeze one end of both into the outlet pipe of the water pump. Bend both of them in opposite directions and glue them in place such that water flows from both the straws and falls just a little ahead of the rotating mop (look at the pictures). Don't forget to put some tape where the straws are connected so the water doesn't leak.

Step 9: Upload the Code
Upload the Code
Remove the Rx and Tx cables from arduino before uploading!

Connect the board to a pc and program it with the code given below. You can make necessary changes.

Make sure you set the correct COM port and Board under Tools.

After it's done, replace the Rx and Tx wires. You'll need to remove them everytime you upload the code.

Code_for_CleanSweep.ino
Download
Step 10: Attach the Battery
Attach the Battery
Attach the Battery
Attach the Battery
View 3 more
For the power source, it's your choice about the type of battery to use. The voltage should be 12V. I would recommend a single lead acid battery or 3x Li-ion 18650, 3.7V each connected in series.

Use some double sided tape or hot glue to keep the battery pack in place. +Ve terminal will go to the transistor circuit from where it will go to Vcc on arduino and to the motor driver circuit. -Ve terminal will be connected to the common Gnd. Use proper battery connectors.

You can even add an On/Off main switch.

If the power LED on the arduino glows, it's all good. Immediately remove the source if LEDs dim rapidly and recheck all the connections. Do not use a very high voltage else the regulator on the board may overheat.

Step 11: Configure the App and Connect
Configure the App and Connect
Configure the App and Connect
Configure the App and Connect
Configure the App and Connect
Go to the google play store and get this app called 'Bluetooth Serial Controller' which lets you set your own control buttons and commands.

After opening the app, click on 'settings' and then 'visibility'

Turn off visibility for buttons 5, 9, 12 as we won't be needing them.

Next, go on the 'names' icon so set the display names for each button. Make them short, 3-4 letters.

For example, look at the names I set above.

Now under the 'commands' option, set the following commands (without quotes) for each button (they are case sensitive):

Button 1 (FWD): 'F'
Button 2 (BCK): 'B'
Button 3 (LFT): 'L'
Button 4 (RGT): 'R'
Button 6 (MPON): 'M'
Button 7 (MPOF): 'm'
Button 8 (PMP): 'P'
Button 10 (RUP): 'U'
Button 11 (RDWN): 'u'
Button 13 (S1): '1'
Button 14 (S2): '2'
Button 15 (S3): '3'
Button 16 (S4): '4'
Under the 'stop commands' section in 'commands' itself, you need to set the following stop commands ONLY for the buttons mentioned below:

Button 1: 'S'
Button 2: 'S'
Button 3: 'S'
Button 4: 'S'
Button 8: 'p'
This means that example if button 2 isn't pressed, the command 'S' will be sent which will stop the robot.

To connect the robot, first pair up the bluetooth module named 'HC-05' or other. Password will be '0000' or '1234'

Then connect the paired up module via the app.

Press and check all the buttons on the app one by one....


Reference Link:
https://www.instructables.com/CleanSweep-the-Floor-Cleaning-Robot/#step11
