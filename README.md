
####latest 8/4/23
### 0 merge conflics with v4.04


general.ini added:
DBGConsoleOn=true

engine.ini added:
[LoadingScreen/Debug]
DisableVideos=true


modAutoConsumeFoodMenu
modAutoEnhanceGearMenu
modAutoLootMenu
modBaseHorseControlsCE
modBetterThanIconsFull_ENG
modColoredMapMarkers_AQO   (set priority over AQO)
modContainerGlow
modDisableFallDMG
modEnhancedCloseCamera
modEnhancedHerbalism
modEqualPrice
modFishlungForeverDiveNG
modFTFA
modGermaniaOne
modGwent-max_bet5000
modHideSaveMessageNG_v404
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


###also

containerglow.xml mod invisible mod menu text fix:

fix
<Group id="ModContainerGlow" displayName="Mods.lego.containerglow">
was
<Group id="ModContainerGlow" displayName="Mods.lego.containerglow" tags="customNames;customDisplayName">














//////
//////old
//////

Enable console add DBGConsoleOn=true in bin\config\base\general.ini 

set Ultra textures then add TextureMipBias=0 under [Rendering] in Documents\The Witcher 3\user.settings

.xml goes in user_config_matrix\pc folder

merge the edited code correctly should be easy enough just select the edited code to the merged from A or B files, absolute camera requires new code i edited below 

modAbsoluteCamera31 / modAbsoluteCameraMenu.xml / Script Merger / LINE 3860ish of r4Player.ws conflict: if ( theGame.IsFocusModeActive() && aCamera.IsOn && theGame.GetInGameConfigWrapper().GetVarValue('FriendlyFocus', 'ffEnableZoomEffect'))
https://www.nexusmods.com/witcher3/mods/856

modZColorfulActionLog / Script Merger 
https://www.nexusmods.com/witcher3/mods/4524

modZActionLog / modActionLog.xml / Script Merger     
https://www.nexusmods.com/witcher3/mods/934

modFriendlyFocus / modFriendlyFocus.xml / Script Merger
https://www.nexusmods.com/witcher3/mods/4261

modAutoLootMenu / AHDAutoLootConfig.xml 
https://www.nexusmods.com/witcher3/mods/1996

modSortEverything / modSortEverything.xml
https://www.nexusmods.com/witcher3/mods/1710

modAbsoluteHorseControl / input.settings changes
https://www.nexusmods.com/witcher3/mods/1411

modExtendedViewDistanceNonAO_VanillaWater
https://www.nexusmods.com/witcher3/mods/3082

modFastTravelFromRoach
https://www.nexusmods.com/witcher3/mods/1684

modHDReworkedProject
https://www.nexusmods.com/witcher3/mods/1021

modnostory
https://www.nexusmods.com/witcher3/mods/816

modUltraGore2
https://www.nexusmods.com/witcher3/mods/519

modz_noplayerlight
https://www.nexusmods.com/witcher3/mods/2414

modNoQuickSaveMessage
https://www.nexusmods.com/witcher3/mods/4948

modOver9000
https://www.nexusmods.com/witcher3/mods/3
