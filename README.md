UI Toggle
@MEMBER 
local ScreenGui = Instance.new("ScreenGui")
local Toggle = Instance.new("TextButton")
    
ScreenGui.Name = "ScreenGui"
ScreenGui.Parent = game.CoreGui
    
Toggle.Name = "Toggle"
Toggle.Parent = ScreenGui
Toggle.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Toggle.BorderSizePixel = 0
Toggle.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)
Toggle.Size = UDim2.new(0, 50, 0, 50)
Toggle.Font = Enum.Font.SourceSans
Toggle.Text = "S"
Toggle.TextColor3 = Color3.fromRGB(1,255,252)
Toggle.TextSize = 50.000
Toggle.Draggable = true
Toggle.MouseButton1Down:connect(function()
    game.CoreGui:FindFirstChild("Name CoreGui").Enabled = not game.CoreGui:FindFirstChild("Name CoreGui").Enabled
end)
do
if game:GetService("CoreGui"):FindFirstChild("Name CoreGui") then
      game:GetService("CoreGui").StringUI:Destroy()
   end
end
