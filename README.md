-- // Services
local AkaliNotif = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kinlei/Dynissimo/main/Scripts/AkaliNotif.lua"))()
local Workspace = game:GetService("Workspace")
local Players = game:GetService("Players")

-- // Variables
local GetEaster = Workspace:WaitForChild("Easter001!")
local GetPlayer = Players.LocalPlayer
local HuntCFrame = CFrame.new(-65, 3, 58)
local fireclickdetector = fireclickdetector or fire_click_detector

local Notify = AkaliNotif.Notify;
function notify(text,duration)
Notify({
Description = text;
Title = "BrookhavenRP";
Duration = duration;
});
end

-- // Easy Farming
notify("BrookhavenRP CandyFarm made by CJStyles123...",15)
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.FallingDown, false)
fireclickdetector(game:GetService("Workspace")["EasterSign001!"].Model.Easy.ClickDetector)
repeat task.wait() until GetEaster:FindFirstChild("HalloweenHuntEazy")
if GetEaster["HalloweenHuntEazy"] then
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, false)
for i,v in pairs(GetEaster.HalloweenHuntEazy:GetChildren()) do
repeat task.wait()
GetPlayer.Character.HumanoidRootPart.CFrame = v.Middle.CFrame
until v.Middle.EggTouched.Value == true
end
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, true)
notify("CandyFarm: <b><font color=\"rgb(245, 205, 48)\">Easy</font></b> mode has been Finished.",15)
end

repeat task.wait() until not GetPlayer.PlayerGui:FindFirstChild("HalloweenHuntGuiEazy")

-- // Medium Farming
fireclickdetector(game:GetService("Workspace")["EasterSign001!"].Model.Medium.ClickDetector)
repeat task.wait() until GetEaster:FindFirstChild("HalloweenHuntMedium")
if GetEaster["HalloweenHuntMedium"] then
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, false)
for i,v in pairs(GetEaster.HalloweenHuntMedium:GetChildren()) do
repeat task.wait()
GetPlayer.Character.HumanoidRootPart.CFrame = v.Middle.CFrame
until v.Middle.EggTouched.Value == true
end
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, true)
notify("CandyFarm: <b><font color=\"rgb(245, 205, 48)\">Medium</font></b> mode has been Finished.",15)
end

repeat task.wait() until not GetPlayer.PlayerGui:FindFirstChild("HalloweenHuntGuiMedium")

-- // Hard Farming
fireclickdetector(game:GetService("Workspace")["EasterSign001!"].Model.Hard.ClickDetector)
repeat task.wait() until GetEaster:FindFirstChild("HalloweenHuntHard")
if GetEaster["HalloweenHuntHard"] then
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, false)
for i,v in pairs(GetEaster.HalloweenHuntHard:GetChildren()) do
repeat task.wait()
GetPlayer.Character.HumanoidRootPart.CFrame = v.Middle.CFrame
until v.Middle.EggTouched.Value == true
end
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, true)
notify("CandyFarm: <b><font color=\"rgb(245, 205, 48)\">Hard</font></b> mode has been Finished.",15)
end

repeat task.wait() until not GetPlayer.PlayerGui:FindFirstChild("HalloweenHuntGuiHard")

-- // Extreme Farming
fireclickdetector(game:GetService("Workspace")["EasterSign001!"].Model.Extreme.ClickDetector)
repeat task.wait() until GetEaster:FindFirstChild("HalloweenHuntExtreme")
if GetEaster["HalloweenHuntExtreme"] then
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, false)
for i,v in pairs(GetEaster.HalloweenHuntExtreme:GetChildren()) do
repeat task.wait()
GetPlayer.Character.HumanoidRootPart.CFrame = v.Middle.CFrame
until v.Middle.EggTouched.Value == true
end
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, true)
notify("CandyFarm: <b><font color=\"rgb(245, 205, 48)\">Extreme</font></b> mode has been Finished.",15)
end

repeat task.wait() until not GetPlayer.PlayerGui:FindFirstChild("HalloweenHuntGuiExtreme")

-- // Insane Farming
fireclickdetector(game:GetService("Workspace")["EasterSign001!"].Model.Insane.ClickDetector)
repeat task.wait() until GetEaster:FindFirstChild("HalloweenHuntInsane")
if GetEaster["HalloweenHuntInsane"] then
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, false)
for i,v in pairs(GetEaster.HalloweenHuntInsane:GetChildren()) do
repeat task.wait()
GetPlayer.Character.HumanoidRootPart.CFrame = v.Middle.CFrame
until v.Middle.EggTouched.Value == true
end
GetPlayer.Character.Humanoid:SetStateEnabled(Enum.HumanoidStateType.Seated, true)
notify("CandyFarm: <b><font color=\"rgb(245, 205, 48)\">Insane</font></b> mode has been Finished.",15)
end
repeat task.wait() until not GetPlayer.PlayerGui:FindFirstChild("HalloweenHuntGuiInsane")
notify("CandyFarm: Thank <b><font color=\"rgb(245, 205, 48)\">You</font></b> for using this script! - CJStyles123",15)
