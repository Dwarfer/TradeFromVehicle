## [TFV] TradeFromVehicle  
### Version 2.0
####  
> http://epochmod.com/forum/index.php?/topic/11931-release-tradefromvehicle-version-20-is-here/

**Credits**:
Based on Csus original trade from vehicle version 2. 90% of the work is his so all credits to him please. I have just modded for Coins and ConfigTrader plus a little TAX :-),

**Requirements**:

   Notepad++ 
	http://notepad-plus-plus.org/
   Notepad++ sqf addon 
	http://www.armaholic.com/page.php?id=8680
   PBO Manager
	http://www.armaholic.com/page.php?id=16369
   Epoch 1.0.4+ Server

**Difficulty** :

    Some knowledge of Epoch Server & Mission file locations
    How to use PBO manager to unpack and pack PBO files
    Easy : ~ 5 minutes

--------------------------
Installation
--------------------------
Installation -
    Put these files into your mission PBO.
    Open up your 'init.sqf' file and find this line of code, around line 75 -
       if (!isDedicated) then {
    Place the following line of code just below that -
       ExecVM "TradeFromVehicle Version 2.0\setup\init.sqf";

Total Size: ~37kb

Setup -
    Head into the setup folder and open up the init.sqf.
    Modify the 5 variables there to suit your needs.