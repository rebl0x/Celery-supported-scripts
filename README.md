# Celery-Supported Scripts
!CELERY IS ENDED, REPO WILL REMAIN UP! <br>
Without using a custom UNC script, here is a list of loadstrings Celery can run by default. Unless your custom Celery has auto-detect loadstring, use the code below to run loadstrings. Add it to the top before the loadstring. <br>

Celery by default is context 3. UNC should be higher now, the main UNC script is broken so we have no way of knowing yet. <br>
(Removed Supported UI-Libs since it broke again and Ill have to re-write for the new celery update) <br>

**Scripts**
- Infinite Yield
  ```lua
  loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/6dd93df4-e15c-4b63-b894-4ca54c2a74a7)

- Dex v2
  ```lua
  loadstring(game:HttpGet("https://raw.githubusercontent.com/tickwares/loadstringtest/main/dexs"))()
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/080db141-5285-4f05-ab22-9d74a9960f14)

- Btools
  ```lua
  backpack = game:GetService("Players").LocalPlayer.Backpack

  hammer = Instance.new("HopperBin")
  hammer.Name = "Hammer"
  hammer.BinType = 4
  hammer.Parent = backpack

  cloneTool = Instance.new("HopperBin")
  cloneTool.Name = "Clone"
  cloneTool.BinType = 3
  cloneTool.Parent = backpack

  grabTool = Instance.new("HopperBin")
  grabTool.Name = "Grab"
  grabTool.BinType = 2
  grabTool.Parent = backpack
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/0057ebaf-f25e-48ab-b79e-3ad29228491c)

- ShatterVast Admin
  ```lua
  loadstring(game:httpGet("https://raw.githubusercontent.com/TERIHAX/Scripts/main/Universal/Admin%20Scripts/ShatterVast.lua"))()
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/2365f615-31d7-41a9-bedd-d09970b3f7fc)

- Fe Animations GUI
  ```lua
  loadstring(game:HttpGet("https://raw.githubusercontent.com/rebl0x/Scripts/main/Fe%20Animations"))()
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/afb98b68-e4f5-44b0-8801-214ae91a8a1c)

- Teams Based ESP
  ```lua
  loadstring(game:HttpGet("https://pastebin.com/raw/1UZ8Yynd"))()
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/148d8817-8417-483e-9286-cc5cfcfecc46)

- Caesar Admin
  ```lua
  loadstring(game:HttpGet("https://raw.githubusercontent.com/byteveil/celery-compatible-scripts/main/scripts/caeser-admin.lua"))()
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/191c5279-2a35-4f25-8849-22985cc8670f)

- Simple Admin
  ```lua
  loadstring(game:HttpGet("https://raw.githubusercontent.com/byteveil/celery-compatible-scripts/main/scripts/simple-admin.lua"))()
  ```
![image](https://github.com/rebl0x/Celery-supported-scripts/assets/169552876/1df5c3af-5d42-4f0d-8e31-fa2cff8848b3)

**Unsupported Scripts**
- Dex V1 ❌ (Needs rewrite to work, doing that as of 14/05/2024)
- Dex V3 ❌ (no getobjects support)
- Dex V4 ❌ (no getobjects support)
- Dex V5 ❌ (Loadstring: failed)
- SecureDarkDexV3 ❌ (Attempted to call nil value)
- SentinelDex ❌ (Loadstring: Failed)
- Unnamed ESP ❌ (This might just be an error on my client since I've seen it run on Celery before)
- Game Rejoin Script ❌ (Causes Roblox to crash)
- MrSpy ❌ (Loadstring: failed)
- Remote2Script ❌ (Loadstring: failed)
- SimpleSpy ❌ (Attempted to call nil value)
- CMD-X ❌ (Attempted to call nil value)
- RevizAdminV2 ❌ (Loadstring: Failed)

**FAQ:**
- Why does it freeze when I click execute? 
  - It's just loading. Wait around a minute max and your script should be loaded.

**Note**
- You can make your own Celery exploit right now.
  [Link to YouTube Video](https://www.youtube.com/watch?v=82u6qf7zn68)

Repository maintained by _t38. (Contributions from byteveil)
