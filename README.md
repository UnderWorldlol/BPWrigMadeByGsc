while true do
	for i,v in pairs(game.Players:GetPlayers()) do
		if v.Name ~= game.Players.LocalPlayer.Name then
			game:GetService("ReplicatedStorage").RemoteEvent:FireServer(30, v)
		end
	end
	wait(0.003)
end
