UNIVERSE BIOS 4.0 for the MVS/AES NeoGeo system
-----------------------------------------------


  homepage = http://www.universebios.com
  email    = info@universebios.com


WARNING
-------
I TAKE NO RESPONSIBILITY FOR ANY DAMAGE CAUSED TO YOUR MVS OR AES HARDWARE WHILE
INSTALLING OR USING THE UNIVERSE BIOS. WHILE THE BIOS HAS BEEN FULLY TESTED ON THIS
HARDWARE YOU USE IT AT YOUR OWN RISK.

THE UNIVERSE BIOS HAS BEEN DESIGNED FOR NON COMMERCIAL USERS OF MVS AND AES HARDWARE
ONLY. USING THE UNIVERSE BIOS IN AN ARCADE ENVIRONMENT CAN RESULT IN LOSS OF REVENUE
DUE TO CUSTOMERS OBTAINING FREE CREDITS AND CHEATING. ALTHOUGH THE UNIVERSE BIOS HAS
FEATURES TO HELP STOP THIS FROM HAPPENING I CANNOT BE HELD RESPONSIBLE FOR ANY LOSS
OF REVENUE. DO NOT USE THE UNIVERSE BIOS IN AN ARCADE ENVIRONMENT TO BE SURE.


TERMS OF USE
------------
You can use the UNIVERSE BIOS as long as you own original genuine NeoGeo hardware.
Failure of this may result in you the user violating international copyright laws.
New program code within the UNIVERSE BIOS is (c) Razoola, original BIOS program
code remains copyrighted to SNK.

  DO NOT REVERSE ENGINEER, ALTER OR CHANGE THE UNIVERSE BIOS DATA OR CODE IN ANY WAY.

  DO NOT PROVIDE A SERVICE OFFERING THE UNIVERSE BIOS ON EPROM OR OTHER PHYSICAL
  FORMAT (FREE OR FOR PROFIT).

  DO NOT DISTRIBUTE OR SELL AN ELECTRONIC BINARY VERSION OF THE UNIVERSE BIOS,
  YOU WILL BE LIABLE IF YOU DO SO.


TERMS OF USE (FREE VERSION)
---------------------------
The free UNIVERSE BIOS version is intended for personal use only, you may use it if
you already own an original NeoGeo and you agree to the following terms;

  THAT YOU OWN AN ORIGINAL NEOGEO MVS, NEOGEO AES OR CD SYSTEM.

  THE UNIVERSE BIOS WILL BE FOR YOUR SOLE PERSONAL USE ONLY.

  NOT TO DISTRIBUTE THE UNIVERSE BIOS IN ANY WAY (PHYSICAL OR DIGITAL).

  NOT TO INCLUDE THE UNIVERSE BIOS IN ANY PRODUCT THAT IS SOLD.

  NOT TO SELL THE UNIVERSE BIOS ON EPROM (OR ANY OTHER PHYSICAL MEDIUM).

  NOT TO ALTER THE UNIVERSE BIOS IMAGE FILE IN ANY WAY.

  NOT TO HOLD ME RESPONCIBLE FOR ANY DAMAGE CAUSED BY USING THE UNIVERSE BIOS.


DONATIONS
---------
Although the UNIVERSE BIOS is free, if you find it useful then please consider donating
to help the cause. More information can be found on the official UNIVERSE BIOS homepage.


---------------------------------------------------------------------------------


INTRODUCTION
------------

The UNIVERSE BIOS is for owners of MVS or AES hardware that want an easy way
to change country region or between Arcade or Console mode on boot. Also included
are other features that are not normally possible using the standard MVS bios.

The UNIVERSE BIOS is also designed to give easy access to things like inserting
coins, test mode and memory card management when using the joystick ports only.
Of course the BIOS still allows standard operation too. 


  MAIN FEATURES
  -------------

  - The ability to quickly and easily change operation from MVS to AES. Play your
    favourite games as the home console version enabling all the extra gameplay
    options that come with some games.

  - The ability to quickly and easily change country region (great for games that
    disable blood under USA region).

  - Access to the DEBUG DIP's and DEVELOPER mode.

  - Want unlimited lives or energy... Then cheat in games using the built in
    cheat engine which currently holds over 1570 cheats!!!

  - If you are not happy with the cheats already there then you can patch
    directly into memory any place you like adding your own.

  - Jukebox player where one can listen to game music without sound FX from
    gameplay over the top. Nice option if you want to create MP3's.

  - A ROM CRC32 check where you can confirm a games program roms are good.

  - True USA region support (correct coin display on bottom left and right of
    screen in the same way a true USA BIOS does. You can even force coins to
    register on the 2up side even in a cab with one coin chute only.
  
  - Arcade VS-MODE support which is known to be in the version 6 JAPAN bios.
    Turn this feature on via hard dip 2.

  - PC-2-NEO which gives the ability to upload and download data from the
    system using a cable which can be easily built. 

  Other features
  --------------

  - Remapping of coin switches to select buttons and visa versa. This allows a SNK
    joypad pad to do everything.

  - Once region and operation mode is set the BIOS will remember settings until you
    change them again.

  - Access to the standard Memory Card Utility no matter what Mode the BIOS is in
    (one could never access this menu with the normal MVS BIOS).

  - Access to the standard controller test (was in the AES bios only).

  - Access to Test Mode on boot without the need of wiring the Test Mode JAMMA pins
    or fiddling with DIP's.

  - Enhancements to the TEST MODE menu and hardware test screens.

  - Console mode lockout protection removed from latest games when running on MVS
    hardware (bypasses the red warning screens).

  - Arcade mode lockout protection removed from latest games when running on AES
    hardware (bypasses the red warning screens).

  - Look at internal memory with the built in memory viewer. This is handy for
    tracking faults with slots that don't work (multislot hardware) or carts
    that simply won't start.

  - The ability to soft reboot the system without the need of powering off and on.

  - PICKnMIX (161in1 required), see homepage for more information.


HARDWARE REQUIREMENTS
---------------------
The UNIVERSE BIOS has been designed to work on all MVS hardware types (SLOT1 and
MULTISLOT) and AES hardware. Saying that installation difficulty varies depending
on the actual MVS / AES model you have. See the notes below which correspond
to your hardware type for details. 

  - MV-1, MV-1A(CH), MV-1F(S/T), MV-1FZ, MV-(2F/4F/6F)
 
      MVS models in this category are by far the easiest to install the UNIVERSE BIOS
      on. No soldering is required because the BIOS should already be in a socket.
      If you can follow simple instructions you can install a UNIVERSE BIOS on these.

  - MV-1AX, MV-1ACHX 

      This model is known to have the bios soldered to the PCB. Follow the AES install
      information below. 

  - MV-1B and MV-1C

      These MVS models contain a BIOS that is known to be soldered to the PCB,
      the chip size is also different than that used in other MVS models.
      Because of this the MV-1B and MV-1C are very difficult to install the
      UNIVERSE BIOS on and you should not attempt to install unless you are
      very skilled with a soldering iron.

  - AES system

      The A.E.S system contains a BIOS that is known to be soldered to the PCB,
      saying that the actual chip used is of a standard DIP size. There are two
      different methods of installing the UNIVERSE BIOS. One involves removing
      the old bios and fitting a socket which is the preferred method, info on
      the other can be found at http://unibios.free.fr/piggyback/. You should
      not attempt to install unless you are skilled with a soldering iron.


---------------------------------------------------------------------------------


USING THE UNIVERSE BIOS (MVS only)
----------------------------------
The first time a MVS system is switched on after UNIVERSE BIOS installation the
system will default to EURO region and ARCADE operation mode. The BootUp HW Test
option will be disabled by default also. You can change any of these settings to
your desired setup at any time by following the information in this manual.

  Important Notes
  ---------------
  If the systems backup SRAM battery is dead any changed settings will be lost on
  power down and the default settings will be reloaded. I would suggest recharging
  or replacing the onboard battery in this situation.

  The backup SRAM is totally cleared the first time the UNIVERSE BIOS is run on a
  MVS system, this is to ensure compatibility.


USING THE UNIVERSE BIOS (AES only) 
----------------------------------
Because the AES system has no backup SRAM the system will use the memory card to
store the systems region and operation mode settings. This info is then read once
at power on, it’s not read again after using the system reset button or soft reset
option. If a memory card is not present the system will default to EURO region and
CONSOLE operation mode on power up, you can then change this as required once you
reach the splash screen.

  Important Notes
  --------------- 
  The hardware test will keep looping until you release its button code. The screen
  flashes each time the hardware check loops itself.

  Hard DIP’s are all set in the off position and cannot be changed.

  When in ARCADE mode you cannot disable developer mode.


Accessing Menus
---------------
The following codes should be used while the splash screen is showing or held during
system power up (splash disabled). Button codes will only work on player 1 controls. 

  A+B+C   = Main UNIVERSE BIOS Menu
  A+B+C+D = Memory Card Manager
  B+C+D   = Test mode (MVS only)
  B+C+D   = Hardware Test (AES only)

  (Use 2up controller for the code below)

  A+B+C+D = Controller Test (AES only)


The following codes are available in game only, they will not work if you have disabled
the in game menu (general bios settings).

  START+SELECT = In Game Menu
  START+COIN   = In Game Menu
  START+A+B+C  = In Game Menu


The Main Menu
-------------
To navigate the UNIVERSE BIOS menu you will need to use player 1 controls,
button (A) is used as select, (C) to exit. Here is a list of all available
options along with a small description.

  Region Settings
  ---------------
  This is where you choose your region and operation mode of the BIOS. Any settings
  made on this screen are permanently saved until you decide to change them.

  General Settings (MVS only)
  ---------------------------
  Like the region settings these setting are also saved until changed.

  - Disable BootUp HW Test
      This option forces the UNIVERSE BIOS to skip some hardware tests at power on,
      it makes booting faster but you have no guarantee the system is in full working
      order. This option is on by default. 

  - Disable In Game Menu
      This option disables the in game menu when enabled.

  - Disable Input Crossing
      When enabled this option will disable the input crossing feature.

  - Enable Cabinet Fixes 
      When enabled 1Up (A) and (B) buttons will act as game select buttons during attract
      mode on multislot hardware. This option also registers a coin entered into a cab
      with only one coin chute to the 2Up side if 2Up (START) is held down while coin is
      inserted. Only works in ARCADE mode while 2 coin counters are drawn on screen.

  - Disable Splash Screen
      This option disables the splash screen at startup when enabled.

  - Enable Arcade Protect
      This setting is designed to allow the Universe Bios to be run easier in an arcade
      environment. When enabled either the TEST MODE button must also be pressed or
      hard DIP 1 must be ON for button codes at the splash screen to work. This setting
      also forces the system to reset if a game should crash instead of giving an error.

  Game SoftDIP Settings (AES only)
  --------------------------------
  Here you can change game settings like the amount of lives given per game, amount of
  time rounds lasts or enable blood for example. Note that Soft DIP’s are reset on
  changing the country region so always select your region setup before editing any
  soft DIP’s.

  GameCart CRC Check
  ------------------
  Here you can check that a games program data is correct by using the CRC32 algorithm.
  The screen will display the GAME ID and CRC32 for each memory region used. The result is
  then checked against an internal database to confirm it’s good. Possible messages
  resulting from this check are;

  OK	-  CRC32 Good
  NG	-  CRC32 Bad
  ??	-  CRC32 not in database

  DO NOT take the above output as 100% accurate as some CRC32 values in the database are
  probably wrong (bad dumps etc). If your game does give a different CRC32 than what’s
  expected then please email the details to us (info@universebios.com).

  Jukebox Music Player
  --------------------
  Here you can listen to music from games. Each tune or sound is assigned a sound code.
  By selecting different codes you will hear different tunes or game fx.

  PC-2-NEO
  --------
  This feature allows you to send and receive data from the NeoGeo using a cable that is
  connected to the 2UP joystick port. Using this feature gives one the ability to run
  your own code on the system or backup memory cards for example.

  This feature should be considered beta at this point but is known to work. Please
  visit the official homepage for more information on how to build the cable or
  download the needed PC software.


The In Game Menu
----------------
To navigate the In Game menus use player one controls and button (A) to select. Not doing
anything for a short period will cause the screen to blank while idle. This feature
prevents monitor burn if using the In Game menu to pause games. Available options are.

  The Cheat Database
  ------------------
  Everything is quite straight forward here although using cheats can cause adverse game
  effects. For example, if you experience game lockups when using a cheat try turning it
  off which may allow the game to continue and then enable it again later. Cheats can also
  cause GFX issues, most notably at the end for energy bars. On MULTISLOT hardware any
  active cheats will be disabled when changing game, they will not be restored automatically.

  Debug DIP Settings
  ------------------
  These settings are more advanced. Debug DIPS do different things depending on the game,
  unless you know what your doing it’s best to leave them alone although experimenting won’t
  cause damage. If a cheat is enabled that uses a games debug dip address you will see it
  via a highlighted number under the DIP value.

  Patch Memory
  ------------
  Here you can manually choose addresses in the NeoGeo memory space and patch byte values
  there. For example by placing different values into 0x320000 you can change any currently
  playing music. You can also use this feature for cheats and other stuff.

  Last menu option (selectable)
  -----------------------------
  The final menu setting is changeable, do this by moving the joystick left or right once
  highlighted. Possible options are;

    Soft Reboot System
    Menu Color Changer 
    Main Memory Viewer	
    Video RAM Viewer
    PC-2-NEO


Input Crossing
--------------
This feature gives you the ability to use the joystick ports (if the system has them) and
the JAMMA connector for things they weren’t initially designed for. Here’s a breakdown on
how it works.

  When using the joystick ports (if the system has them) the select buttons will insert
  coins when pressed if running in arcade mode. On MULTISLOT hardware this is disabled
  when more than one game found (ensures correct game changing operation).

  When using the JAMMA connection for joystick control the coin switches (for getting credits)
  become player 1 and player 2 select buttons when in console mode (see known issues).

  On a MULTISLOT system the joystick port select buttons and JAMMA connector select game
  pins do the same thing (by hardware design). This means you can use the game select buttons
  as player 1 and player 2 select buttons too.

  On a MULTISLOT system game selecting is only available during the attract mode sequence
  when in console mode.


---------------------------------------------------------------------------------


BURNING THE UNIVERSE BIOS ONTO EPROM
------------------------------------

The UNIVERSE BIOS requries a 27C1024 type EPROM, simply burn the UNIVERSE BIOS image
onto it and then put it in place of the original BIOS on your NeoGeo hardware.


OBTAINING THE UNIVERSE BIOS ON EPROM
------------------------------------

If you would like the UNIVERSE BIOS provided on EPROM because you don't have the ability
to do it yourself then visit the official homepage for information on how to get one.


---------------------------------------------------------------------------------
