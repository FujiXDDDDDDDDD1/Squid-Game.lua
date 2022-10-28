local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
    
    
    
    local Window = Library.CreateLib("Fu Kang Hub", "BloodTheme")
    -- MAIN
    local Teleports = Window:NewTab("Teleports")
    local TeleportsSection = Teleports:NewSection("Teleports")
    TeleportsSection:NewLabel("Lobby")
    TeleportsSection:NewButton("Teleport Game Play", "Fu Kang Hub", function()
	local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(-30,5,-105)
    end)
    
    TeleportsSection:NewLabel("Teleport")
    
    TeleportsSection:NewButton("Teleport 1", "Fu Kang Hub", function()
    local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(-129.8,15.0625,-660.95) -- 1.yan 2.yukarı aşağı 3.ileri geri
    end)

    TeleportsSection:NewButton("Teleport 2", "Fu Kang Hub", function()
    local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(-27.325, -70.025, -572.438) -- 1.yan 2.yukarı aşağı 3.ileri geri

    end)

    TeleportsSection:NewButton("Teleport 3", "Fu Kang Hub", function()
    local plr = game.Players.LocalPlayer
	local char = plr.Character
	char.HumanoidRootPart.CFrame = CFrame.new(106.6, -67.9122, -90.12) -- 1.yan 2.yukarı aşağı 3.ileri geri

    end)

    TeleportsSection:NewButton("Teleport 4", "Fu Kang Hub", function()
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
     PlayerSection:NewSlider("Walkspeed", "Fu Kang Hub", 250, 16, function(v)
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v
    end)

    local settings = Window:NewTab("Settings")
    local settingsSection = settings:NewSection("Settings")
settingsSection:NewKeybind("Hide UI", "Fu kang Hub", Enum.KeyCode.RightShift, function()
	Library:ToggleUI()
end)
