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
