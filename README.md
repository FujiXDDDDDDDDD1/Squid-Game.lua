local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
    
    
    
    local Window = Library.CreateLib("Fu Kang Hub", "DarkTheme")
    -- MAIN
    local Teleports = Window:NewTab("Teleports")
    local TeleportsSection = Teleports:NewSection("Teleports")
    TeleportsSection:NewLabel("works in the lobby")
    TeleportsSection:NewButton("Teleport Game Play", "Teleports to the game starting point in the lobby", function()
	local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(-30,5,-105)
    end)
    
    TeleportsSection:NewLabel("Works in game")
    
    TeleportsSection:NewButton("Teleport Safe", "Please do not teleport as soon as the game starts", function()
    local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(-129.8,15.0625,-660.95) -- 1.yan 2.yukarı aşağı 3.ileri geri
    end)

    TeleportsSection:NewButton("Teleport Dormitory", "teleports to the dormitory", function()
    local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(-27.325, -70.025, -572.438) -- 1.yan 2.yukarı aşağı 3.ileri geri

    end)

    TeleportsSection:NewButton("Teleport End Parkour", "teleport to the end of parkour", function()
    local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(106.6, -67.9122, -90.12) -- 1.yan 2.yukarı aşağı 3.ileri geri

    end)

    TeleportsSection:NewButton("Teleport All Glass", "breaking the whole glass and teleporting to the opposite side", function()
   	local plr = game.Players.LocalPlayer
	local char = plr.Character
    local spt = 0.1
	char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-355.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-355.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-344.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-344.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-333.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-333.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-322.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-322.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-311.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-311.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-300.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-300.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-299.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-299.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-288.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-288.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-277.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-277.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-266.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-266.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-255.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-255.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-244.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-244.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-233.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-233.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-222.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-222.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-332,-125.6,-211.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-125.6,-211.425)
    wait(spt)
    char.HumanoidRootPart.CFrame = CFrame.new(-342,-118.6,-189.425)    -- 1.yan 2.yukarı aşağı 3.ileri geri
    end)
    
    local Player = Window:NewTab("Player")
    local PlayerSection = Player:NewSection("Player")
     PlayerSection:NewSlider("Walkspeed", "Changes the walkspeed", 250, 16, function(v)
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v
    end)

    PlayerSection:NewButton("Finish the candy", "removes sugar from mold", function()
   game:GetService("ReplicatedStorage").Remotes.SugarHoneycomb:FireServer(true)
    end)

local pulling = true
PlayerSection:NewToggle("Automatic rope pulling", "presses the button for you", function(state)
pulling = state
 while wait(0.05) do
if pulling == true then
     game:GetService("ReplicatedStorage").TugRemote:FireServer() 
     else
     break   
    end
 end
 end)

    PlayerSection:NewButton("Kill All", "You must have a baseball bat", function()
   for i=1,15 do
   for i,v in next,game.Players:GetPlayers()do
       if v~=game.Players.LocalPlayer then
           game.ReplicatedStorage.Remotes.Replication:FireServer(v.Character.Humanoid,10)
       end
   end
end
    end)
    local settings = Window:NewTab("Settings")
    local settingsSection = settings:NewSection("Settings")
settingsSection:NewKeybind("Menu on/off", "Menu on/off", Enum.KeyCode.RightShift, function()
	Library:ToggleUI()
end)
