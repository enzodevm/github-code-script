-- LocalScript

-- Referência ao jogador local
local player = game.Players.LocalPlayer

-- Função para teletransportar o personagem
local function teleportCharacter()
    -- Verifica se o jogador tem um personagem
    if player.Character then
        -- Define a nova posição para teleportar
        local newPosition = Vector3.new(0, 50, 0) -- Altere as coordenadas conforme necessário

        -- Teleporta o personagem
        player.Character:SetPrimaryPartCFrame(CFrame.new(newPosition))
    end
end

-- Função para ativar a opção
local function onOptionActivated()
    teleportCharacter()
end

-- Conecte a função ao evento de clique (por exemplo, se você estiver usando um botão)
local button = script.Parent -- Supondo que o LocalScript esteja dentro de um botão
button.MouseButton1Click:Connect(onOptionActivated)
OrionLib:Init()

OrionLib:MakeNotification({
    Name = "Asho Hub",
    Content = "Loading Config Complete!!",
    Image = "rbxassetid://119980140458596",
    Time = 5
    OrionLib:Init()

OrionLib:MakeNotification({
    Name = "Asho Hub",
    Content = "Loading Config Complete!!",
    Image = "rbxassetid://119980140458596",
    Time = 5
})
})
