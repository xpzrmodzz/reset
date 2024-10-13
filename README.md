-- Function to handle player's death
local function forceResetAction()
    local player = game.Players.LocalPlayer
    
    -- Vérifie si le personnage et le humanoïde existent
    if player.Character and player.Character:FindFirstChild("Humanoid") then
        player.Character.Humanoid.Health = 0  -- Force le reset en mettant la santé à zéro
    end
end

-- Exemple d'utilisation
forceResetAction()  -- Appelle la fonction pour forcer le reset
