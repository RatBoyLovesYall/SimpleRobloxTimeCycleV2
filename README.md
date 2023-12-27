# SimpleRobloxTimeCycleV2

--time changer
local mam --minutes after midnight
local timeShift = 0.1 --how many minutes you shift every "tick"
local waitTime = 1/30 --length of the tick
local pi = math.pi

while true do
	--time changer
	mam = game.Lighting:GetMinutesAfterMidnight() + timeShift
	game.Lighting:SetMinutesAfterMidnight(mam)
	mam = mam/60

	--tick
	wait(waitTime)
end
