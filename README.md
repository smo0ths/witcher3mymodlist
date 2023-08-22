#### updated 8/22/23


general.ini added:
```python
DBGConsoleOn=true
```

engine.ini added:
```python
[LoadingScreen/Debug]
DisableVideos=true
```

dx12user.settings/user.settings added:

```python
[Rendering]                    (find)
DisableBigCameraLights=true    (add)
DisableSmallCameraLights=false (add)
DisableAllCameraLights=false   (add)

[Streaming/Textures]           (find)
CinematicModeMipBias=-1        (changed)
UseMipRefiner=true             (add)
```

latest modAutoLootMenu v4.3.4 has merge conflicts in r4Player.ws with modEnhancedCloseCamera here is the fix:

```python
line 15261~ copy/paste
	//+++EnhancedCloseCamera+++
	public var EnhancedCloseCamera : CEnhancedCloseCamera;
	
	public function GetEnhancedCloseCamera(): CEnhancedCloseCamera
	{
		return EnhancedCloseCamera;
	}
	
	timer function EnableCameraShake(dt : float, id : int)
	{
		if (GetEnhancedCloseCamera().GetCameraShake())
		{
			GetEnhancedCloseCamera().StartCameraShake();
		}
		else if (GetEnhancedCloseCamera().IsCameraShakeActive())
		{
			GetEnhancedCloseCamera().StopCameraShake();
		}
	}
	//---EnhancedCloseCamera---
	timer function InitAHDAutoLoot(dt : float, id : int) // AutoLootMenu++ IMPORTANT DO NOT CHANGE
	{
		GetAutoLootConfig().InitAutoLootConfig();
		GetAutoLootNotificationManager().Reset();
	}
	
	public function GetAutoLootConfig() : CAHDAutoLootConfig { return AutoLootConfig; }
	public function GetAutoLootNotificationManager() : CAHDAutoLootNotificationManager { return AutoLootNotificationManager; }
	
	timer function TrueAutoLootMode( dt : float, id : int )
	{
		GetAutoLootConfig().GetFeatureManager().TryAreaLooting("true_autoloot_mode");
		AddTimer('TrueAutoLootMode', GetAutoLootConfig().GetTrueAutoLootTime());
	}// AutoLootMenu-- IMPORTANT DO NOT CHANGE
}
ending at line 15295~
```

### mods

```python
modAutoEnhanceGearMenu
modAutoLootMenu
modBaseHorseControlsCE
modBetterThanIconsFull_ENG
modColoredMapMarkers_AQO   (set priority over AQO)
modContainerGlow
modDisableFallDMG
modDisableSoftLock
modEnhancedCloseCamera
modEnhancedHerbalism
modEqualPrice
modFishlungForeverDiveNG
modFTFA
modGermaniaOne
modGwent-max_bet5000
modhealthren   (Noncombat Health Regen)
modHideSaveMessageNG_v404
modhpregen   (Noncombat Health Regen)
modMapQuestObjectivesFull
modMissingCardTracker
modMoreMoneyForTraders
modMultipleQuickSave
modNTakTime
modPJ002_BalancedITMLVLs
modSortEverything
modSXPM
modTheTwoGwentStoresNG
modTurnOnTheLights
modUltraGore2NG
modUnlimitedDurability
```

---

eventually:
```python
teleport to map pin   (the old simple mod)
Extend Potion Duration   (this one just needs an update)
add links
```

---
