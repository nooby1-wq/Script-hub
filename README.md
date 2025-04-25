--// Theme Settings
local Theme = {
	MainBackground = Color3.fromRGB(20, 20, 20),
	Sidebar = Color3.fromRGB(30, 30, 30),
	Button = Color3.fromRGB(45, 45, 45),
	Text = Color3.fromRGB(255, 255, 255),
	Stroke = Color3.fromRGB(100, 100, 100)
}

--// Load GUI
local player = game.Players.LocalPlayer
local screenGui = Instance.new("ScreenGui", player:WaitForChild("PlayerGui"))
screenGui.Name = "XtensHub"
screenGui.ResetOnSpawn = false

--// Main Frame
local mainFrame = Instance.new("Frame", screenGui)
mainFrame.Size = UDim2.new(0, 420, 0, 320)
mainFrame.Position = UDim2.new(0.3, 0, 0.25, 0)
mainFrame.BackgroundColor3 = Theme.MainBackground
Instance.new("UICorner", mainFrame)

--// Top Bar
local topBar = Instance.new("Frame", mainFrame)
topBar.Size = UDim2.new(1, 0, 0, 30)
topBar.BackgroundColor3 = Theme.Sidebar
topBar.BorderSizePixel = 0
topBar.Name = "TopBar"

local title = Instance.new("TextLabel", topBar)
title.Size = UDim2.new(1, -60, 1, 0)
title.Position = UDim2.new(0, 10, 0, 0)
title.Text = "xtentacion_fan Hub"
title.BackgroundTransparency = 1
title.Font = Enum.Font.SourceSansBold
title.TextSize = 14
title.TextColor3 = Theme.Text
title.TextXAlignment = Enum.TextXAlignment.Left

-- Minimize Button
local minimizeBtn = Instance.new("TextButton", topBar)
minimizeBtn.Size = UDim2.new(0, 20, 0, 20)
minimizeBtn.Position = UDim2.new(1, -50, 0.5, -10)
minimizeBtn.Text = "_"
minimizeBtn.Font = Enum.Font.SourceSansBold
minimizeBtn.TextSize = 18
minimizeBtn.BackgroundColor3 = Theme.Button
minimizeBtn.TextColor3 = Theme.Text
Instance.new("UICorner", minimizeBtn)

-- Close Button
local closeBtn = Instance.new("TextButton", topBar)
closeBtn.Size = UDim2.new(0, 20, 0, 20)
closeBtn.Position = UDim2.new(1, -25, 0.5, -10)
closeBtn.Text = "X"
closeBtn.Font = Enum.Font.SourceSansBold
closeBtn.TextSize = 14
closeBtn.BackgroundColor3 = Theme.Button
closeBtn.TextColor3 = Theme.Text
Instance.new("UICorner", closeBtn)

--// Sidebar (Tab Holder)
local tabHolder = Instance.new("Frame", mainFrame)
tabHolder.Position = UDim2.new(0, 0, 0, 30)
tabHolder.Size = UDim2.new(0, 100, 1, -30)
tabHolder.BackgroundColor3 = Theme.Sidebar
Instance.new("UICorner", tabHolder)

--// Content Frame
local contentFrame = Instance.new("Frame", mainFrame)
contentFrame.Position = UDim2.new(0, 110, 0, 40)
contentFrame.Size = UDim2.new(1, -120, 1, -50)
contentFrame.BackgroundTransparency = 1

--// Tab Frames
local tabs = {
	Universal = Instance.new("Frame"),
	MM2 = Instance.new("Frame"),
	BloxFruit = Instance.new("Frame")
}

for name, frame in pairs(tabs) do
	frame.Size = UDim2.new(1, 0, 1, 0)
	frame.Visible = false
	frame.BackgroundTransparency = 1
	frame.Parent = contentFrame

	local layout = Instance.new("UIListLayout", frame)
	layout.Padding = UDim.new(0, 5)
end

local function switchTab(tabName)
	for name, frame in pairs(tabs) do
		frame.Visible = (name == tabName)
	end
end

--// Icon Tabs
local function createTabButton(name, iconId)
	local btn = Instance.new("TextButton", tabHolder)
	btn.Size = UDim2.new(1, 0, 0, 40)
	btn.BackgroundColor3 = Theme.Button
	btn.Text = ""
	btn.BorderSizePixel = 0

	local icon = Instance.new("ImageLabel", btn)
	icon.Size = UDim2.new(0, 20, 0, 20)
	icon.Position = UDim2.new(0, 10, 0.5, -10)
	icon.Image = "rbxassetid://" .. iconId
	icon.BackgroundTransparency = 1

	local text = Instance.new("TextLabel", btn)
	text.Position = UDim2.new(0, 35, 0, 0)
	text.Size = UDim2.new(1, -40, 1, 0)
	text.BackgroundTransparency = 1
	text.Text = name
	text.Font = Enum.Font.SourceSansBold
	text.TextSize = 14
	text.TextColor3 = Theme.Text
	text.TextXAlignment = Enum.TextXAlignment.Left

	Instance.new("UICorner", btn)
	local stroke = Instance.new("UIStroke", btn)
	stroke.Color = Theme.Stroke
	stroke.Thickness = 1

	btn.MouseButton1Click:Connect(function()
		switchTab(name)
	end)
end

-- Tabs
createTabButton("Universal", "6035047390")
createTabButton("MM2", "6031624245")
createTabButton("BloxFruit", "6031075931")
switchTab("Universal")

-- Safe Loader
local function safeLoad(url)
	pcall(function()
		loadstring(game:HttpGet(url))()
	end)
end

-- Button Creator
local function createButton(parent, name, callback)
	local button = Instance.new("TextButton")
	button.Size = UDim2.new(1, 0, 0, 32)
	button.BackgroundColor3 = Theme.Button
	button.TextColor3 = Theme.Text
	button.Text = name
	button.Font = Enum.Font.SourceSansBold
	button.TextSize = 14
	button.Parent = parent
	button.AutoButtonColor = true

	local corner = Instance.new("UICorner", button)
	local stroke = Instance.new("UIStroke", button)
	stroke.Color = Theme.Stroke
	stroke.Thickness = 1

	button.MouseButton1Click:Connect(callback)
end

-- Universal Tab
createButton(tabs.Universal, "Fly", function()
	safeLoad("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt")
end)
createButton(tabs.Universal, "Invisible", function()
	safeLoad("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Invisible%20Gui")
end)
createButton(tabs.Universal, "Wall Walk", function()
	safeLoad("https://pastebin.com/raw/zXk4Rq2r")
end)
createButton(tabs.Universal, "Reverse Script", function()
	safeLoad("https://mscripts.vercel.app/scfiles/reverse-script.lua")
end)

-- MM2 Tab
createButton(tabs.MM2, "OverDrive", function()
	safeLoad("https://raw.githubusercontent.com/Universal-Script/ODH/refs/heads/main/Overdrive-H")
end)
createButton(tabs.MM2, "Kill All (Murderer Only)", function()
	safeLoad("https://pastefy.app/uIN86D8E/raw")
end)
createButton(tabs.MM2, "Forge Hub", function()
	safeLoad("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua")
end)

-- BloxFruit Tab
createButton(tabs.BloxFruit, "Redz", function()
	safeLoad("https://pastefy.app/dmU9ZSwh/raw")
end)
createButton(tabs.BloxFruit, "HoHo Hub", function()
	safeLoad("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI")
end)
createButton(tabs.BloxFruit, "Auto Bounty", function()
	safeLoad("https://pastefy.app/eQDjzB6t/raw")
end)

-- Minimize / Restore
local isMinimized = false
minimizeBtn.MouseButton1Click:Connect(function()
	isMinimized = not isMinimized
	contentFrame.Visible = not isMinimized
	tabHolder.Visible = not isMinimized
	minimizeBtn.Text = isMinimized and "+" or "_"
end)

-- Close Button + Open Button
closeBtn.MouseButton1Click:Connect(function()
	mainFrame.Visible = false
	openBtn.Visible = true
end)

-- Open Button
local openBtn = Instance.new("TextButton", screenGui)
openBtn.Size = UDim2.new(0, 120, 0, 35)
openBtn.Position = UDim2.new(0.01, 0, 0.9, 0)
openBtn.Text = "Open xtens Hub"
openBtn.BackgroundColor3 = Theme.Sidebar
openBtn.TextColor3 = Theme.Text
openBtn.Font = Enum.Font.SourceSansBold
openBtn.TextSize = 14
openBtn.Visible = false
Instance.new("UICorner", openBtn)

openBtn.MouseButton1Click:Connect(function()
	mainFrame.Visible = true
	openBtn.Visible = false
end)

-- Dragging with TopBar only
local dragging, dragInput, dragStart, startPos
topBar.InputBegan:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseButton1 then
		dragging = true
		dragStart = input.Position
		startPos = mainFrame.Position
		input.Changed:Connect(function()
			if input.UserInputState == Enum.UserInputState.End then
				dragging = false
			end
		end)
	end
end)

topBar.InputChanged:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseMovement then
		dragInput = input
	end
end)

game:GetService("UserInputService").InputChanged:Connect(function(input)
	if input == dragInput and dragging then
		local delta = input.Position - dragStart
		mainFrame.Position = UDim2.new(
			startPos.X.Scale,
			startPos.X.Offset + delta.X,
			startPos.Y.Scale,
			startPos.Y.Offset + delta.Y
		)
	end
end)
