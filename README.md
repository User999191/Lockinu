local library = loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/ShaddowScripts/Main/main/Library"))()

local Main = library:CreateWindow("Celex Updated! ! !","Crimson")

local tab = Main:CreateTab("AimBot")
local tab2 = Main:CreateTab("Misc")

tab:CreateButton("CamLock V1",function()
       loadstring(game:HttpGet("https://raw.githubusercontent.com/User999191/Lockin/main/README.md", true))()
end)

tab:CreateButton("CamLock V2",function()
       loadstring(game:HttpGet("https://raw.githubusercontent.com/User999191/Lockinv2/main/README.md", true))()
end)

tab:CreateButton("Celex tracer Custom lock 0.1",function()
       loadstring(game:HttpGet("https://raw.githubusercontent.com/User999191/Lockiv3/main/README.md", true))()
end)

tab:CreateButton("Q tool Custom",function()
       --credits to thatsnotmatt#2602
getgenv().keytoclick = "Q"
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = keytoclick
tool.Activated:connect(function()
    local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, keytoclick, false, game)
end)
tool.Parent = game.Players.LocalPlayer.Backpack
wait(0.2)
local AkaliNotif = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kinlei/Dynissimo/main/Scripts/AkaliNotif.lua"))();
local Notify = AkaliNotif.Notify;
Notify({
Description = "Celex";
Title = "This Celex has V4 button but soon";
Duration = 7;
});
mouse = game.Players.LocalPlayer:GetMouse()

end)

tab:CreateButton("C tool Custom",function()
       --credits to thatsnotmatt#2602
getgenv().keytoclick = "c"
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = keytoclick
tool.Activated:connect(function()
    local vim = game:service("VirtualInputManager")
vim:SendKeyEvent(true, keytoclick, false, game)
end)
tool.Parent = game.Players.LocalPlayer.Backpack
wait(0.2)
local AkaliNotif = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kinlei/Dynissimo/main/Scripts/AkaliNotif.lua"))();
local Notify = AkaliNotif.Notify;
Notify({
Description = "Celex";
Title = "This Celex has V4 button but soon";
Duration = 7;
});
mouse = game.Players.LocalPlayer:GetMouse()

end)

tab:CreateCheckbox("Anti Slow Reload",function(a)
while wait(0) do
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 27
end
end)
