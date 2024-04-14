- -- This script is a basic template for an anime game in Roblox

-- Variables
local player = game.Players.LocalPlayer
local humanoid = player.Character:WaitForChild("Humanoid")

-- Function to play an anime animation
local function playAnimeAnimation(animationId)
    local animation = Instance.new("Animation")
    animation.AnimationId = "rbxassetid://" .. animationId
    humanoid:LoadAnimation(animation):Play()
end

-- Function to handle player input
local function onKeyPress(input)
    if input.KeyCode == Enum.KeyCode.Q then
        -- Play a running animation
        playAnimeAnimation(1234567890) -- Replace with the animation ID of your choice
    elseif input.KeyCode == Enum.KeyCode.E then
        -- Play a jumping animation
        playAnimeAnimation(9876543210) -- Replace with the animation ID of your choice
    end
end

-- Connect the function to the player's input
player:GetMouse().KeyDown:Connect(onKeyPress)

-  ...
-  ...
-  ...
-  ...
- : ...
- ⚡ : ...

<!---

--->
