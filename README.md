--luau
Mueda = workspace.MUEDA

PontosPleyer = 0


Mueda.Touched:Connect(function(hit)
	
	local PosicaoX = math.random(-5,5)
	
	local PosicaoZ = math.random(-5,5)
	
	Mueda.Position = Vector3.new(PosicaoX,3,PosicaoZ)
	
	task.wait(0.5)
	
	PontosPleyer = PontosPleyer + 1
	
	print("Pontos:", PontosPleyer)
	
end)
