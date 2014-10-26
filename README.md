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

Setup -
    Head into the setup folder and open up the init.sqf.
    Modify the 5 variables there to suit your needs.
    
	TFV_ATFV = true;   // Allow trading from vehicles?
	TFV_ATFB = true;   // Allow trading from backpack?
	TFV_ACC =  false;   // Allow combining currency? This attempts to sort the player's money into as few items as possible, e.g. 10 * 10oz Gold into 1 * Gold Briefcase.
	TFV_WIPS =    5;   // *How many weapons can be sold per stage of trading? Each stage of trading is the length of time to perform the standard trading animation.
	TFV_MIPS =    8;   // *How many magazines can be sold per stage of trading?
	TFV_ATIS = true;   // Allow toolbelt items to be sold? Toolbelt items are classed as weapons and will be sold without warning when weapons are sold. Keys will ALWAYS be safe.
	TFV_COINS = true;  //Coins System
	TFV_DEBUG = false;  //Debug

	// This is in a * Multiplier to 100*1 = 100, 100*0.5 = 50, 100*0.75 = 75 25% Tax,100*0.25 = 25 75% Tax.
	TFV_TAX = true;
	TFV_TAXFV = 0.75; // Tax From Veichle 25%
	TFV_TAXFVT = "25"; // Dispay Tax Veichle (lazy code TBH)
	TFV_TAXFB= 0.85; // Tax From Backpack 15%
	TFV_TAXFBT= "15"; // Dispay Tax Backpack (lazy code TBH)

If you have DZE_ConfigTrader enabled this will automaticlaly work. *hopefully* 
