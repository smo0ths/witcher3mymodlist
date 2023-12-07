#### updated 12/7/23

##### 1440p scaling (DLSS/FSR2/TAAU/XeSS) 58%/67%/70% resolution scale (balance/quality) -1/-0.5 (recommended negative LOD bias)

##### 4k scaling (DLSS/FSR2/TAAU/XeSS) 50% resolution scale (performance) -1.5/-1 (recommended negative LOD bias)

---

general.ini added:
```python
DBGConsoleOn=true
```

engine.ini added:
```python
[LoadingScreen/Debug]
DisableVideos=true
```

---

dx12user.settings/user.settings added:

```python
[Rendering]                    (find)
DisableBigCameraLights=true    (add)
DisableSmallCameraLights=false (add)
DisableAllCameraLights=false   (add)
TextureMipBias=-1.5            (changed)

[Streaming/Textures]           (find)
CinematicModeMipBias=-1.5      (changed)
UseMipRefiner=false            (add cost 12 fps if true)
```

---

### mods

```python
modAutoEnhanceGearMenu
modAutoLootMenu
modBetterThanIconsFull_ENG
modColoredMapMarkers_AQO   (set priority over AQO)
modContainerGlow
modDisableFallDMG
modEnhancedCloseCamera
modEnhancedHerbalism
modEnhancedTargeting
modEqualPrice
modFishlungForeverDiveNG
modFTFA
modGermaniaOne
modGwent-max_bet5000
modHideSaveMessageNG_v404
modImprovedHorseControls
modMapQuestObjectivesFull
modMissingCardTracker
modMoreMoneyForTraders
modMultipleQuickSave
modNTakTime
modPJ002_BalancedITMLVLs
modSmoothGUI
modSortEverything   (set priority over SmoothGUI)
modstackpotionsdurationbonus
modSXPM
modTheTwoGwentStoresNG
modTurnOnTheLights   (bugs out quest where you manually light things)
modTweaks
modUltraGore2NG
modUnlimitedDurability
```
