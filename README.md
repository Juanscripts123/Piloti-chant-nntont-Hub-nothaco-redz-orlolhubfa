local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/Library-ui/refs/heads/main/Redzhubui"))()

local Window = redzlib:MakeWindow({
    Title = "Lolkid Hub",
    SubTitle = "Luscaa and lolkid Team",
    SaveFolder = "Lusca"
})

Window:AddMinimizeButton({
    Button = { Image = "rbxassetid://112013915649339", BackgroundTransparency = 0 },
    Corner = { CornerRadius = UDim.new(35, 5) },
})


local LocalTab = Window:MakeTab({"local jogador", "paper"})

local Section = LocalTab:AddSection({"Velocidade, jump"})


LocalTab:AddTextBox({
    Name = "Velocidade ",
    Description = "Set the walking speed of your player",
    PlaceholderText = "Coloca Velocidade vida (normal: 16)",
    Callback = function(Value)
        local speed = tonumber(Value)
        if speed and game.Players.LocalPlayer.Character then
            game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = speed
            print("Velocidade cu set to: " .. speed)
        else
            print("Cy")
        end
    end
})

LocalTab:AddTextBox({
    Name = "Jump Power",
    Description = "Coloca o Pulo",
    placeholdertext = "Coloca a força aqui vidoca (default: 50)",
    Callback = function(Value)
        local jumpPower = tonumber(Value)
        if jumpPower and game.Players.LocalPlayer.Character then
            game.Players.LocalPlayer.Character.Humanoid.JumpPower = jumpPower
            print("Pulo set to: " .. jumpPower)
      else
            print("Cu")
        end
    end
})

local LocalTab = Window:MakeTab({"informações", "settings "})

local Section = LocalTab:AddSection({"aqui é informações"})
LocalTab:AddTextBox({
    Name = "o script está em beta terá bug",
    Description = "uma coisinha ",
    placeholdertext = "você pode colocar uma avaliação aqui",
    Callback = function(Value)
        local jumpPower = tonumber(Value)
        if jumpPower and game.Players.LocalPlayer.Character then
            game.Players.LocalPlayer.Character.Humanoid.JumpPower = jumpPower
            print("Pulo set to: " .. jumpPower)
      else
            print("Cu")
        end
    end
})

local LocalTab = Window:MakeTab({"precisa de ajuda ?", "settings "})

local Section = LocalTab:AddSection({"entre em https://discord.gg/8n4nydNWUE ou https://discord.gg/GsAavzhT9b"})

local LocalTab = Window:MakeTab({"créditos?", " home "})

local Section = LocalTab:AddSection({"quem fez isso foi o Lucaas do chaos hub mais isso é uma fan made"})

local LocalTab = Window:MakeTab({"som all", "paper"})

local Section = LocalTab:AddSection({"depois vou adicionartralaleioo"})
