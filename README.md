#### updated 8/4/23
### 0 merge conflics with v4.04


general.ini added:
```python
DBGConsoleOn=true
```

engine.ini added:
```python
[LoadingScreen/Debug]
DisableVideos=true
```
### mods

```python
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
```

---

### also

containerglow.xml makes mod menu words invisible so you fix it with this:

```python
fix
<Group id="ModContainerGlow" displayName="Mods.lego.containerglow">
was
<Group id="ModContainerGlow" displayName="Mods.lego.containerglow" tags="customNames;customDisplayName">
```

---
