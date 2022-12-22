local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("boss hub", "Synapse")

-- MAIN
local Main = Window:NewTab("Main")
local MainSection = Main:NewSection("auto farm")


MainSection:NewButton("auto sell", "autos sells", function()
    while wait() do

        game:GetService("ReplicatedStorage").Remotes.SellPower:InvokeServer()
        end
end)

MainSection:NewToggle("super-speed", "be fast", function(state)
    if state then
         game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 120
    else
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
    end
end)

MainSection:NewButton("auto click", "if you die re click it and dont pull out weapon or it will stop so you have to do it again", function()
    while wait() do

local args = {
    [1] = game:GetService("Players").LocalPlayer.Character["Gold Naginata"]
}

game:GetService("ReplicatedStorage").Remotes.Power:FireServer(unpack(args))
end
end)


--LOCAL PLAYER
local Player = Window:NewTab("Player")
local PlayerSection = Player:NewSection("Player")

PlayerSection:NewSlider("Speed!", "gives you speed", 500, 16, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

PlayerSection:NewSlider("jumppower", "jump high", 350, 50, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)


--Other
local Other = Window:NewTab("Other")
local OtherSection = Other:NewSection("Other")

OtherSection:NewButton("chat-spoofer", "types messages from the user you wont", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/ant-7802/--/main/straightmilk.lua'))()
end)

OtherSection:NewButton("infinite-yield", "commands", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)

