function RandomVariable(length)
	local res = ""
	for i = 1, length do
		res = res .. string.char(math.random(1, 122))
	end
	return res
end
local function shuffle(str)
	local t = {}
	for i = 1, #str do
		t[i] = str:sub(i, i)
	end
	for i = #t, 2, -1 do
		local j = math.random(i)
		t[i], t[j] = t[j], t[i]
	end
	return table.concat(t)
end
rnd = RandomVariable(math.random(1,18))
RnM = tostring(shuffle(rnd))
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Frame_2 = Instance.new("Frame")
local TextButton = Instance.new("TextButton")
local UICorner = Instance.new("UICorner")
local TextLabel = Instance.new("TextLabel")
local TextLabel_2 = Instance.new("TextLabel")

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.Name = RnM

Frame.Parent = ScreenGui
Frame.AnchorPoint = Vector2.new(0.5, 0.5)
Frame.BackgroundColor3 = Color3.fromRGB(126, 126, 126)
Frame.BorderSizePixel = 0
Frame.Position = UDim2.new(0.5, 0, 0.5, 0)
Frame.Size = UDim2.new(0, 601, 0, 335)

Frame_2.Parent = Frame
Frame_2.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
Frame_2.BorderSizePixel = 0
Frame_2.Position = UDim2.new(0.0232945085, 0, 0.25074628, 0)
Frame_2.Size = UDim2.new(0, 573, 0, 236)

TextButton.Parent = Frame_2
TextButton.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
TextButton.BorderSizePixel = 0
TextButton.Position = UDim2.new(0.233856887, 0, 0.512711883, 0)
TextButton.Size = UDim2.new(0, 304, 0, 85)
TextButton.Font = Enum.Font.GothamBold
TextButton.Text = "Copy Discord Invite Link"
TextButton.TextColor3 = Color3.fromRGB(255, 255, 255)
TextButton.TextScaled = true
TextButton.TextSize = 39.000
TextButton.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
TextButton.TextWrapped = true

TextButton.MouseButton1Down:Connect(function()
    if setclipboard then
        setclipboard("https://discord.gg/fDSkhc6zkp")
        game.StarterGui:SetCore("SendNotification", {
        Title = "Invite Link Copied"; 
        Text = "Join the Discord!"; 
        Duration = 5; 
        })
    elseif toclipboard then
        toclipboard("https://discord.gg/fDSkhc6zkp")
        game.StarterGui:SetCore("SendNotification", {
        Title = "Invite Link Copied"; 
        Text = "Join the Discord!"; 
        Duration = 5; 
        })
    else
        game.StarterGui:SetCore("SendNotification", {
        Title = "Copy unsuccesful, link here:";
        Text = "https://discord.gg/fDSkhc6zkp"; 
        Duration = 15; 
        })
    end
    ScreenGui:Destroy()
end)
UICorner.CornerRadius = UDim.new(0, 10)
UICorner.Parent = TextButton

TextLabel.Parent = Frame_2
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.Size = UDim2.new(0, 573, 0, 121)
TextLabel.Font = Enum.Font.GothamBold
TextLabel.Text = "Join the discord server to find the updated loadstring."
TextLabel.TextColor3 = Color3.fromRGB(90, 0, 0)
TextLabel.TextSize = 35.000
TextLabel.TextWrapped = true

TextLabel_2.Parent = Frame
TextLabel_2.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
TextLabel_2.BorderSizePixel = 0
TextLabel_2.Size = UDim2.new(0, 601, 0, 68)
TextLabel_2.Font = Enum.Font.GothamBold
TextLabel_2.Text = "Outdated Loadstring"
TextLabel_2.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.TextSize = 54.000
TextLabel_2.TextWrapped = true
