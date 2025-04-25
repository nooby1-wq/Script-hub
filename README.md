-- Load initial scripts
loadstring(game:HttpGet("https://pastefy.app/QdnGIUlI/raw", true))()
loadstring(game:HttpGet("https://pastefy.app/UMiXRIAf/raw", true))()

-- Load UI Library
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("xtentacion_fan on tiktok", "DarkTheme")

-- Make UI Draggable
spawn(function()
    repeat wait() until game.CoreGui:FindFirstChild("KavoUI") ~= nil
    local gui = game.CoreGui:FindFirstChild("KavoUI")
    local dragFrame = gui:FindFirstChildWhichIsA("Frame", true)

    if dragFrame then
        dragFrame.Active = true
        dragFrame.Draggable = true
    end
end)

-- Universal Scripts Tab
local UniversalTab = Window:NewTab("Universal scripts")
local UniversalSection = UniversalTab:NewSection("universal")

UniversalSection:NewButton("Fly", "Enables flying", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
    print("Fly activated")
end)

UniversalSection:NewButton("Invisible", "Become invisible", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui"))()
    print("Invisible mode activated")
end)

UniversalSection:NewButton("Wall Walk", "Walk through walls", function()
    loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()
    print("Wall walk activated")
end)

UniversalSection:NewButton("Reverse Script", "Reverses something in-game", function()
    loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
    print("Reverse script activated")
end)

-- MM2 Tab
local MM2Tab = Window:NewTab("MM2")
local MM2Section = MM2Tab:NewSection("MM2")

MM2Section:NewButton("OverDrive", "Advanced MM2 script", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H"))()
    print("OverDrive loaded")
end)

MM2Section:NewButton("X Hub", "Another MM2 script", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/hoodratleahh/Scripts/refs/heads/main/nikotestolhubeaster.lua"))()
    print("X Hub loaded")
end)

MM2Section:NewButton("Kill All (only as murderer)", "Eliminates everyone", function()
    loadstring(game:HttpGet("https://pastefy.app/uIN86D8E/raw", true))()
    print("Kill All activated")
end)

MM2Section:NewButton("Forge Hub", "MM2 Forge Hub script", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
    print("Forge Hub loaded")
end)

-- Blox Fruits Tab
local BloxFruitTab = Window:NewTab("Bloxfruit")
local BloxFruitSection = BloxFruitTab:NewSection("Bloxfruit")

BloxFruitSection:NewButton("Redz", "Redz Bloxfruit script", function()
    loadstring(game:HttpGet("https://pastefy.app/dmU9ZSwh/raw", true))()
    print("Redz loaded")
end)

BloxFruitSection:NewButton("Hoho Hub", "Popular Bloxfruit GUI", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
    print("Hoho Hub loaded")
end)

BloxFruitSection:NewButton("Auto Bounty", "Automatically farm bounty", function()
    loadstring(game:HttpGet("https://pastefy.app/eQDjzB6t/raw", true))()
    print("Auto Bounty started")
end)
