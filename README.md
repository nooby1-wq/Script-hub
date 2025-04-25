ChatGPT

Log in
You said:
Organize the script:
- Load Rayfield UI
loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Create the main window
local Window = Rayfield:CreateWindow({
	Name = "Multi Game Hub",
	LoadingTitle = "Multi Game Hub",
	LoadingSubtitle = "by your_name_here",
	ConfigurationSaving = {
		Enabled = false
	},
	KeySystem = false
})

-- Universal Scripts Tab
local UniversalTab = Window:CreateTab("Universal Scripts", 4483362458)
UniversalTab:CreateSection("Scripts")

UniversalTab:CreateButton({
	Name = "Fly",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Invisible",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Wall Walk",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Reverse Script",
	Callback = function()
		loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
	end,
})

-- MM2 Scripts Tab
local MM2Tab = Window:CreateTab("MM2", 4483362458)
MM2Tab:CreateSection("MM2 Scripts")

MM2Tab:CreateButton({
	Name = "OverDrive",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H"))()
	end,
})

MM2Tab:CreateButton({
	Name = "X Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/hoodratleahh/Scripts/refs/heads/main/nikotestolhubeaster.lua"))()
	end,
})

MM2Tab:CreateButton({
	Name = "Kill All (Murderer only)",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/uIN86D8E/raw", true))()
	end,
})

MM2Tab:CreateButton({
	Name = "Forge Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
	end,
})

-- Blox Fruits Scripts Tab
local BloxTab = Window:CreateTab("Blox Fruits", 4483362458)
BloxTab:CreateSection("Bloxfruit Scripts")

BloxTab:CreateButton({
	Name = "Redz",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/dmU9ZSwh/raw", true))()
	end,
})

BloxTab:CreateButton({
	Name = "Hoho Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
	end,
})

BloxTab:CreateButton({
	Name = "Auto Bounty",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/eQDjzB6t/raw", true))()
	end,
})

ChatGPT said:
Here's your organized and neatly formatted script for clarity and better maintainability:

lua
Copy code
-- Load Rayfield UI
loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Create the main window
local Window = Rayfield:CreateWindow({
	Name = "Multi Game Hub",
	LoadingTitle = "Multi Game Hub",
	LoadingSubtitle = "by your_name_here",
	ConfigurationSaving = {
		Enabled = false
	},
	KeySystem = false
})

--============================================================
-- Universal Scripts Tab
--============================================================
local UniversalTab = Window:CreateTab("Universal Scripts", 4483362458)
UniversalTab:CreateSection("Scripts")

UniversalTab:CreateButton({
	Name = "Fly",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Invisible",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Wall Walk",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Reverse Script",
	Callback = function()
		loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
	end,
})

--============================================================
-- MM2 Scripts Tab
--============================================================
local MM2Tab = Window:CreateTab("MM2", 4483362458)
MM2Tab:CreateSection("MM2 Scripts")

MM2Tab:CreateButton({
	Name = "OverDrive",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H"))()
	end,
})

MM2Tab:CreateButton({
	Name = "X Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/hoodratleahh/Scripts/refs/heads/main/nikotestolhubeaster.lua"))()
	end,
})

MM2Tab:CreateButton({
	Name = "Kill All (Murderer only)",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/uIN86D8E/raw", true))()
	end,
})

MM2Tab:CreateButton({
	Name = "Forge Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
	end,
})

--============================================================
-- Blox Fruits Scripts Tab
--============================================================
local BloxTab = Window:CreateTab("Blox Fruits", 4483362458)
BloxTab:CreateSection("Bloxfruit Scripts")

BloxTab:CreateButton({
	Name = "Redz",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/dmU9ZSwh/raw", true))()
	end,
})

BloxTab:CreateButton({
	Name = "Hoho Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
	end,
})

BloxTab:CreateButton({
	Name = "Auto Bounty",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/eQDjzB6t/raw", true))()
	end,
})
Let me know if you want to add categories for other games or improve the UI further!


You said:
Add this script:
loadstring(game:HttpGet("https://pastefy.app/QdnGIUlI/raw",true))()

ChatGPT said:
Sure! Just let me know which tab and optionally what name/title you'd like to give this button. For example:

Add to Universal Scripts tab?

Name the button something like "ESP Script", "New Utility", etc.?

If you're not sure, I can place it under Universal Scripts with a default name. Want me to go ahead and do that?


You said:
Don't ace it to the tab place it inside the script

ChatGPT said:
Got it! Here's the updated and organized full script with your new script added. I’ve placed the new loadstring line neatly at the bottom of the script so it's still part of the full execution but not attached to any tab button:

lua
Copy code
-- Load Rayfield UI
loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Create the main window
local Window = Rayfield:CreateWindow({
	Name = "Multi Game Hub",
	LoadingTitle = "Multi Game Hub",
	LoadingSubtitle = "by your_name_here",
	ConfigurationSaving = {
		Enabled = false
	},
	KeySystem = false
})

--============================================================
-- Universal Scripts Tab
--============================================================
local UniversalTab = Window:CreateTab("Universal Scripts", 4483362458)
UniversalTab:CreateSection("Scripts")

UniversalTab:CreateButton({
	Name = "Fly",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Invisible",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Wall Walk",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Reverse Script",
	Callback = function()
		loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
	end,
})

--============================================================
-- MM2 Scripts Tab
--============================================================
local MM2Tab = Window:CreateTab("MM2", 4483362458)
MM2Tab:CreateSection("MM2 Scripts")

MM2Tab:CreateButton({
	Name = "OverDrive",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H"))()
	end,
})

MM2Tab:CreateButton({
	Name = "X Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/hoodratleahh/Scripts/refs/heads/main/nikotestolhubeaster.lua"))()
	end,
})

MM2Tab:CreateButton({
	Name = "Kill All (Murderer only)",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/uIN86D8E/raw", true))()
	end,
})

MM2Tab:CreateButton({
	Name = "Forge Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
	end,
})

--============================================================
-- Blox Fruits Scripts Tab
--============================================================
local BloxTab = Window:CreateTab("Blox Fruits", 4483362458)
BloxTab:CreateSection("Bloxfruit Scripts")

BloxTab:CreateButton({
	Name = "Redz",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/dmU9ZSwh/raw", true))()
	end,
})

BloxTab:CreateButton({
	Name = "Hoho Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
	end,
})

BloxTab:CreateButton({
	Name = "Auto Bounty",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/eQDjzB6t/raw", true))()
	end,
})

--============================================================
-- Extra Script (Standalone)
--============================================================
loadstring(game:HttpGet("https://pastefy.app/QdnGIUlI/raw", true))()
Let me know if you want this script tied to a button later or kept as a background load.


You said:
Add this next to the one I gave earlier:
loadstring(game:HttpGet("https://pastefy.app/UMiXRIAf/raw",true))()

ChatGPT said:
Perfect! Here's your updated and organized script with both standalone scripts at the bottom, side by side, just like you asked:

lua
Copy code
-- Load Rayfield UI
loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Create the main window
local Window = Rayfield:CreateWindow({
	Name = "Multi Game Hub",
	LoadingTitle = "Multi Game Hub",
	LoadingSubtitle = "by your_name_here",
	ConfigurationSaving = {
		Enabled = false
	},
	KeySystem = false
})

--============================================================
-- Universal Scripts Tab
--============================================================
local UniversalTab = Window:CreateTab("Universal Scripts", 4483362458)
UniversalTab:CreateSection("Scripts")

UniversalTab:CreateButton({
	Name = "Fly",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Invisible",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Wall Walk",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Reverse Script",
	Callback = function()
		loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
	end,
})

--============================================================
-- MM2 Scripts Tab
--============================================================
local MM2Tab = Window:CreateTab("MM2", 4483362458)
MM2Tab:CreateSection("MM2 Scripts")

MM2Tab:CreateButton({
	Name = "OverDrive",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H"))()
	end,
})

MM2Tab:CreateButton({
	Name = "X Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/hoodratleahh/Scripts/refs/heads/main/nikotestolhubeaster.lua"))()
	end,
})

MM2Tab:CreateButton({
	Name = "Kill All (Murderer only)",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/uIN86D8E/raw", true))()
	end,
})

MM2Tab:CreateButton({
	Name = "Forge Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
	end,
})

--============================================================
-- Blox Fruits Scripts Tab
--============================================================
local BloxTab = Window:CreateTab("Blox Fruits", 4483362458)
BloxTab:CreateSection("Bloxfruit Scripts")

BloxTab:CreateButton({
	Name = "Redz",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/dmU9ZSwh/raw", true))()
	end,
})

BloxTab:CreateButton({
	Name = "Hoho Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
	end,
})

BloxTab:CreateButton({
	Name = "Auto Bounty",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/eQDjzB6t/raw", true))()
	end,
})

--============================================================
-- Extra Scripts (Standalone)
--============================================================
loadstring(game:HttpGet("https://pastefy.app/QdnGIUlI/raw", true))()
loadstring(game:HttpGet("https://pastefy.app/UMiXRIAf/raw", true))()
Let me know if you want labels, button versions, or if these scripts should only load conditionally!


You said:
Change the name of the gui into xtentacion_fan on tiktok

ChatGPT said:
Done! Here's the updated script with the GUI name changed to "xtentacion_fan on tiktok" across both the window name and loading titles:

lua
Copy code
-- Load Rayfield UI
loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Create the main window
local Window = Rayfield:CreateWindow({
	Name = "xtentacion_fan on tiktok",
	LoadingTitle = "xtentacion_fan on tiktok",
	LoadingSubtitle = "by your_name_here",
	ConfigurationSaving = {
		Enabled = false
	},
	KeySystem = false
})

--============================================================
-- Universal Scripts Tab
--============================================================
local UniversalTab = Window:CreateTab("Universal Scripts", 4483362458)
UniversalTab:CreateSection("Scripts")

UniversalTab:CreateButton({
	Name = "Fly",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Invisible",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Wall Walk",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()
	end,
})

UniversalTab:CreateButton({
	Name = "Reverse Script",
	Callback = function()
		loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
	end,
})

--============================================================
-- MM2 Scripts Tab
--============================================================
local MM2Tab = Window:CreateTab("MM2", 4483362458)
MM2Tab:CreateSection("MM2 Scripts")

MM2Tab:CreateButton({
	Name = "OverDrive",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H"))()
	end,
})

MM2Tab:CreateButton({
	Name = "X Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/hoodratleahh/Scripts/refs/heads/main/nikotestolhubeaster.lua"))()
	end,
})

MM2Tab:CreateButton({
	Name = "Kill All (Murderer only)",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/uIN86D8E/raw", true))()
	end,
})

MM2Tab:CreateButton({
	Name = "Forge Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
	end,
})

--============================================================
-- Blox Fruits Scripts Tab
--============================================================
local BloxTab = Window:CreateTab("Blox Fruits", 4483362458)
BloxTab:CreateSection("Bloxfruit Scripts")

BloxTab:CreateButton({
	Name = "Redz",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/dmU9ZSwh/raw", true))()
	end,
})

BloxTab:CreateButton({
	Name = "Hoho Hub",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
	end,
})

BloxTab:CreateButton({
	Name = "Auto Bounty",
	Callback = function()
		loadstring(game:HttpGet("https://pastefy.app/eQDjzB6t/raw", true))()
	end,
})

--============================================================
-- Extra Scripts (Standalone)
--============================================================
loadstring(game:HttpGet("https://pastefy.app/QdnGIUlI/raw", true))()
loadstring(game:HttpGet("https://pastefy.app/UMiXRIAf/raw", true))(
