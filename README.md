
-- Load initial scripts
loadstring(game:HttpGet("https://pastefy.app/QdnGIUlI/raw", true))()
loadstring(game:HttpGet("https://pastefy.app/UMiXRIAf/raw", true))()

-- Load Rayfield UI Library
local Rayfield = loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

local Window = Rayfield:CreateWindow({
    Name = "xtentacion_fan on TikTok",
    LoadingTitle = "xtentacion_fan Hub",
    LoadingSubtitle = "by You",
    ConfigurationSaving = {
        Enabled = false
    },
    Discord = {
        Enabled = false
    },
    KeySystem = false
})

-- Universal Scripts Tab
local UniversalTab = Window:CreateTab("Universal Scripts", 4483362458)
UniversalTab:CreateSection("Universal")

UniversalTab:CreateButton({
    Name = "Fly",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
        print("Fly clicked")
    end
})

UniversalTab:CreateButton({
    Name = "Invisible",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui"))()
        print("Invisible clicked")
    end
})

UniversalTab:CreateButton({
    Name = "Wall Walk",
    Callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()
        print("Wall Walk clicked")
    end
})

UniversalTab:CreateButton({
    Name = "Reverse Script",
    Callback = function()
        loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
        print("Reverse clicked")
    end
})

-- MM2 Tab
local MM2Tab = Window:CreateTab("MM2", 4483362458)
MM2Tab:CreateSection("MM2")

MM2Tab:CreateButton({
    Name = "OverDrive",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H"))()
        print("OverDrive clicked")
    end
})

MM2Tab:CreateButton({
    Name = "Kill All (Murderer Only)",
    Callback = function()
        loadstring(game:HttpGet("https://pastefy.app/uIN86D8E/raw", true))()
        print("Kill all clicked")
    end
})

MM2Tab:CreateButton({
    Name = "Forge Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
        print("Forge Hub clicked")
    end
})

-- BloxFruit Tab
local BloxFruitTab = Window:CreateTab("BloxFruit", 4483362458)
BloxFruitTab:CreateSection("BloxFruit")

BloxFruitTab:CreateButton({
    Name = "Redz",
    Callback = function()
        loadstring(game:HttpGet("https://pastefy.app/dmU9ZSwh/raw", true))()
        print("Redz clicked")
    end
})

BloxFruitTab:CreateButton({
    Name = "HoHo Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
        print("HoHo Hub clicked")
    end
})

BloxFruitTab:CreateButton({
    Name = "Auto Bounty",
    Callback = function()
        loadstring(game:HttpGet("https://pastefy.app/eQDjzB6t/raw", true))()
        print("Auto Bounty clicked")
    end
})
