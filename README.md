# exile_uid-loadout

Step 1:
  Put the folder "uid_loadout" into your Exile.Altis

Step 2:
  Put following code into your Exile.Altis/config.cpp - class CfgExileCustomCode:
```
  ExileServer_object_player_network_createPlayerRequest = "uid_loadout\ExileServer_object_player_network_createPlayerRequest.sqf";
```
Step 3: Put the following code into your @ExileServer/addons/exile_server_config/config.cpp at the bottom:
```
  ///////////////////////////////////////////////////////////////////////
  // UID LOADOUT CONFIGURATION by Jenartor
  ///////////////////////////////////////////////////////////////////////
  class UID_Loadout_Settings{
  	uidLoadoutMode = 1;

  	uids[] =
  	{
  		"YourUID",
      "NextUID",
      "Ithinkyougotthepoint"
  	};

    // ItemList
  	loadOut[] =
  	{
  		"ItemCompass",
  		"ItemMap",
  		"Exile_Item_XM8",
  		"ItemRadio",
  		"Exile_Item_PlasticBottleFreshWater",
  		"ItemGPS",
  		"hgun_P07_F",
  		"16Rnd_9x21_Mag",
  		"16Rnd_9x21_Mag"
  	};
  };
```

Step 4: Pack your .pbo and upload it to your GameServer
Step 5: Start your GameServer
