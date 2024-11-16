
local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
	Name = " 한국 스크립트 | 제작 크리스탈 ",
	LoadingTitle = " 크리스탈 x ",
	LoadingSubtitle = "by 1_F0",
	ConfigurationSaving = {
		Enabled = false,
		FolderName = nil, -- Create a custom folder for your hub/game
		FileName = "Example Hub"
	},

	KeySystem = true, -- Set this to true to use our key system
	KeySettings = {
		Title = "크리스탈 스크립트 ",
		Subtitle = "크리스탈 x ",
		Note = "Key (키 비밀)",
		FileName = "YoutubeHubKey1", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
		SaveKey = false, -- The user's key will be saved, but if you change the key, they will be unable to use your script
		GrabKeyFromSite = true, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
		Key = {"크리스탈"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
	}
})

Rayfield:Notify({
	Title = "크리스탈 허브 스크립트",
	Content = "어피치 GUIi",
	Duration = 5,
	Image = 13047715178,
	Actions = { -- Notification Buttons
		Ignore = {
			Name = "좋아요!",
			Callback = function()
				print("사용자가 확인을 탭했습니다.")
			end
		},
	},
})


local MainTab = Window:CreateTab(" 홈", nil)
local MainSection = MainTab:CreateSection("기본")

local Slider = MainTab:CreateSlider({
	Name = "걷기 스피드 Slider",
	Range = {1, 350},
	Increment = 1,
	Suffix = "Speed",
	CurrentValue = 16,
	Flag = "sliderws", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
	Callback = function(Value)
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = (Value)
	end,
})

local Slider = MainTab:CreateSlider({
	Name = " 점프파워 Slider",
	Range = {1, 350},
	Increment = 1,
	Suffix = "Speed",
	CurrentValue = 16,
	Flag = "sliderjp", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
	Callback = function(Value)
		game.Players.LocalPlayer.Character.Humanoid.JumpPower = (Value)
	end,
})


local Input = MainTab:CreateInput({
	Name =
 "걷기스피드",
	PlaceholderText = "1-500",
	RemoveTextAfterFocusLost = true,
	Callback = function(Text)
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = (Text)
	end,
})


local Input = MainTab:CreateInput({
	Name =
 "점프속도",
	PlaceholderText = "1-500",
	RemoveTextAfterFocusLost = true,
	Callback = function(Text)
		game.Players.LocalPlayer.Character.Humanoid.jump = (Text)
	end,
})


local TPTab = Window:CreateTab("플레이어", nil)
local OtherSection = TPTab:CreateSection("어드민")

local Button1 = TPTab:CreateButton({
   Name = "어드민",
   Callback = function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
       --Teleport1
   end,
})

local OtherSection = TPTab:CreateSection("플라이")

local Button2 = TPTab:CreateButton({
   Name = "플라이 GUI",
   Callback = function()
loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10")()
        --Teleport2
   end,
})

local OtherSection = TPTab:CreateSection("애니메이션")

local Button3 = TPTab:CreateButton({
   Name = "R6 애니메이션 GUI",
   Callback = function()
    loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Energize-10408"))()  
 --Teleport3
   end,
})

local TPTab = Window:CreateTab("플레이어위치", nil)
local OtherSection = TPTab:CreateSection("위치")

 local TPTab = Window:CreateTab("프리즌 라이프", nil)
local OtherSection = TPTab:CreateSection("프리즌")


local Button1 = TPTab:CreateButton({
   Name = "스크립트1",
   Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Denverrz/scripts/master/PRISONWARE_v1.3.txt"))()
        --Teleport1       
   end,
})

local Button2 = TPTab:CreateButton({
   Name = "아직없음2",
   Callback = function()
        --Teleport2
   end,
})

local Button3 = TPTab:CreateButton({
   Name = "아직없음3",
   Callback = function()
        --Teleport3
   end,
})

local Button4 = TPTab:CreateButton({
   Name = "아직없음4",
   Callback = function()
        --Teleport4
   end,
})

local Button5 = TPTab:CreateButton({
   Name = "아직없음5",
   Callback = function()
        --Teleport5
   end,
})


local TPTab = Window:CreateTab("보물선 만들기", nil)
local OtherSection = TPTab:CreateSection("보물선")


local Button1 = TPTab:CreateButton({
   Name = "오토팜",
   Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/Rocks7hub/Rockshub/main/Build.boat"))()
       --Teleport1
   end,
})
