local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("TITLE", "fixk")

-- MAIN
local Tab = Window:NewTab("Main")
local MainSection = Tab:NewSection("Main")


MainSection:NewButton("LocalX", "LocalX님의 스크", function()
    print("Clicked")
end)



--LOCAL PLAYER

MainSection:NewButton("inflnlte YIELD", "free admin", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)

MainSection:NewToggle("super-Human", "speed (120)", function(state)
    if state then
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 120
    else
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 32
    end
end)

MainSection:NewToggle("super-Human", "jump (100)", function(state)
    if state then
        game.Players.LocalPlayer.Character.Humanoid.Jumppower = 100
    else
        game.Players.LocalPlayer.Character.Humanoid.Jumppower = 50
    end
end)

MainSection:NewButton("CMD-X", "free admin 2", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/CMD-X/CMD-X/master/Source",true))()
end)

