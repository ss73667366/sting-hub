local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "스팅 허브",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "로딩중...",
   LoadingSubtitle = "by 스팅",
   Theme = "Default", -- Check https://docs.sirius.menu/rayfield/configuration/themes

   DisableRayfieldPrompts = false,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = false,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Big Hub"
   },

   Discord = {
      Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = "스팅의 스크립트 Hub",
      Subtitle = "환영합니다!",
      Note = "키 : 123", -- Use this to tell the user how to get a key
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = false, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"123"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local mainTab = Window:CreateTab("기본적인것들", nil) -- Title, Image
local mainSection = mainTab:CreateSection("기본적인 것들")

local Button = mainTab:CreateButton({
   Name = "기본적인 허브",
   Callback = function()
  loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "직접만든무적",
   Callback = function()
  -- 무적 스크립트 예시
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

-- 캐릭터의 "Humanoid" 파트 가져오기
local humanoid = character:WaitForChild("Humanoid")

-- 무적 상태를 설정하는 함수
local function makeInvincible()
    humanoid.HealthChanged:Connect(function(health)
        if health < humanoid.MaxHealth then
            humanoid.Health = humanoid.MaxHealth
        end
    end)
end

-- 스크립트 실행
makeInvincible()

   end,
})

local Button = mainTab:CreateButton({
   Name = "SystemBroken",
   Callback = function()
  loadstring(game:HttpGet("https://raw.githubusercontent.com/H20CalibreYT/SystemBroken/main/script"))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "스피드있고다른좋은거많은기본핵-개좋음음-qp",
   Callback = function()
  loadstring(game:HttpGet("https://raw.githubusercontent.com/QP-Community/Roblox-Exploit/main/Sirius"))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "ESP",
   Callback = function()
   loadstring(game:HttpGet('https://raw.githubusercontent.com/ic3w0lf22/Unnamed-ESP/master/UnnamedESP.lua',true))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "Radar",
   Callback = function()
   loadstring(game:HttpGet("https://pastebin.com/raw/7jv0Tnz5"))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "가짜헤드리스",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/scripthubekitten/fakelimitedsv2/main/fakelimitedsv2", true))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "어드민",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/FilteringEnabled/NamelessAdmin/main/Source"))()
   end,
})

local mainTab = Window:CreateTab("프리즌라이프", nil) -- Title, Image
local mainSection = mainTab:CreateSection("프리즌라이프")

local Button = mainTab:CreateButton({
   Name = "프리즌라이프어드민",
   Callback = function()
   loadstring(game:HttpGet("https://scriptblox.com/raw/Prison-Life-Prizz-Admin-14511"))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "프리즌라이프 허브1",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/Denverrz/scripts/master/PRISONWARE_v1.3.txt"))()
   end,
})

local Button = mainTab:CreateButton({
   Name = "프리즌라이프 허브2",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/thaibao/main/TbaohubPrisonLife"))()
   end,
})

local mainTab = Window:CreateTab("배드워즈", nil) -- Title, Image
local mainSection = mainTab:CreateSection("배드워즈")

 local Button = mainTab:CreateButton({
   Name = "배드워즈 vape v4",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/7GrandDadPGN/VapeV4ForRoblox/main/NewMainScript.lua", true))()
   end,
})

local Button = mainTab:CreateButton({
 Name = "Skid Vape",
   Callback = function()
   loadstring(game:HttpGet('https://skidvape.vercel.app/skidloader.lua'))()
   end, 
})

local Button = mainTab:CreateButton({
 Name = "Voidware",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/VapeVoidware/vapevoidware/main/NewMainScript.lua", true))()
   end,    
})

local mainTab = Window:CreateTab("라이벌", nil) -- Title, Image
local mainSection = mainTab:CreateSection("라이벌")

local Button = mainTab:CreateButton({
   Name = "라이벌 총알 자동마춤-서버 바뀔때마다 누르세요",
   Callback = function()
   loadstring(game:HttpGet('https://raw.githubusercontent.com/ThunderScriptSolutions/Misc/refs/heads/main/RivalsSilentAim'))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "SILENT HUB",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/KxGOATESQUE/SilentRivals/main/silentsolara"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Phantom HUB",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/5oxin/Phantom/main/main"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "autowin",
   Callback = function()
   loadstring(game:HttpGet(('https://raw.githubusercontent.com/venoxhh/universalscripts/main/rivals/autowin.lua')))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "autowin2",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/SkibidiCen/RivalsAutoFarmNice/main/Code"))()
   end, 
})

local mainTab = Window:CreateTab("암살자vs보안관", nil) -- Title, Image
local mainSection = mainTab:CreateSection("암살자vs보안관")

local Button = mainTab:CreateButton({
   Name = "살인자vs보안관 가장좋은스크",
   Callback = function()
   loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Update-script-hitbox-9326"))()
   end, 
})

local mainTab = Window:CreateTab("럭키박스", nil) -- Title, Image
local mainSection = mainTab:CreateSection("럭키박스")

local Button = mainTab:CreateButton({
   Name = "BONK HUB",
   Callback = function()
   loadstring(game:HttpGet("https://bonkhubloader.netlify.app",true))()
   end, 
})

local mainTab = Window:CreateTab("아스널", nil) -- Title, Image
local mainSection = mainTab:CreateSection("아스널")

local Button = mainTab:CreateButton({
   Name = "Thunder Client V2 Lite  킬올 있음",
   Callback = function()
   loadstring(game:HttpGet('https://api.luarmor.net/files/v3/loaders/b95e8fecdf824e41f4a030044b055add.lua'))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "qp허브",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/QPScript/Script/main/Arsenal.txt"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Tbao HUB",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/thaibao/main/TbaoHubArsenal"))()
   end, 
})

local mainTab = Window:CreateTab("PETS GO", nil) -- Title, Image
local mainSection = mainTab:CreateSection("PETS GO")

local Button = mainTab:CreateButton({
   Name = "Speed HUB X",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "NS HUB",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/OhhMyGehlee/rel/refs/heads/main/el"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Ather HUB",
   Callback = function()
   loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/2529a5f9dfddd5523ca4e22f21cceffa.lua"))()
   end, 
})

local mainTab = Window:CreateTab("부대테러", nil) -- Title, Image
local mainSection = mainTab:CreateSection("부대테러")

local Button = mainTab:CreateButton({
   Name = "박대근허브 키-FLY",
   Callback = function()
   loadstring(game:HttpGet(('https://raw.githubusercontent.com/SinEunByeol/DGHub/refs/heads/main/NoObfuscator')))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "헙2",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/pudong8452/test_case_h/main/Ray_Free"))()
   end, 
})

local mainTab = Window:CreateTab("블레이드 볼", nil) -- Title, Image
local mainSection = mainTab:CreateSection("블레이드 볼")

local Button = mainTab:CreateButton({
   Name = "FFJ V2",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/FFJ1/Roblox-Exploits/main/scripts/autoparry.lua"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Nexam HUB",
   Callback = function()
   loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/ad08f0225388445dea30f4b42ea0558e.lua"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Expo HUB 키-Expo#1",
   Callback = function()
   loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/ad08f0225388445dea30f4b42ea0558e.lua"))()
   end, 
})

local mainTab = Window:CreateTab("블피", nil) -- Title, Image
local mainSection = mainTab:CreateSection("블피")

local Button = mainTab:CreateButton({
   Name = "블피돈벌이-키-vortex42244",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/Jayson24244/Vortex/refs/heads/main/Bloxfruit", true))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "블피오토팜가능",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/CheemsNhuChiAl/Sotringhuhu/main/StrawberryHubBeta1.35"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "블피허브",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/realredz/BloxFruits/refs/heads/main/Source.lua"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "블피레벨업",
   Callback = function()
   loadstring(game:HttpGet("https://bonkhubloader.netlify.app",true))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "허브2",
   Callback = function()
   loadstring(game:HttpGet(("https://raw.githubusercontent.com/koonpeatch/PeatEX/master/BKHAX/BloxFruits"),true))()
   end, 
})

local mainTab = Window:CreateTab("팬텀포스", nil) -- Title, Image
local mainSection = mainTab:CreateSection("팬텀포스")

local Button = mainTab:CreateButton({
   Name = "Redacted Project허브",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/EdwinS7/RedactedProjectPF/main/Loader.lua"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "homehack",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/dementiaenjoyer/homohack/main/pf_lite.lua"))()
   end, 
})

local mainTab = Window:CreateTab("매드시티", nil) -- Title, Image
local mainSection = mainTab:CreateSection("매드시티")

local Button = mainTab:CreateButton({
   Name = "매드시티1998",
   Callback = function()
   loadstring(game:HttpGet("https://system-exodus.com/scripts/madlads/MadLads.lua",true))()
   end, 
})

local mainTab = Window:CreateTab("머더", nil) -- Title, Image
local mainSection = mainTab:CreateSection("머더")

local Button = mainTab:CreateButton({
   Name = "머더1",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/vertex-peak/vertex/refs/heads/main/loadstring"))()
   end, 
})

local mainTab = Window:CreateTab("머더2", nil) -- Title, Image
local mainSection = mainTab:CreateSection("머더2")

local Button = mainTab:CreateButton({
   Name = "머더2",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/vertex-peak/vertex/refs/heads/main/loadstring"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "ski",
   Callback = function()
   loadstring(game:HttpGet(("https://raw.githubusercontent.com/Yousuck780/mm2/main/mm2"), true))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Vynixu HUB",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/Neon-Fox/roblox-scripts/main/VynixuMM2"))()
   end, 
})

local mainTab = Window:CreateTab("피쉬", nil) -- Title, Image
local mainSection = mainTab:CreateSection("피쉬")

local Button = mainTab:CreateButton({
   Name = "BONK HUB",
   Callback = function()
   loadstring(game:HttpGet("https://bonkhubloader.netlify.app",true))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Rinns HUB",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/kylosilly/femboyware/refs/heads/main/Fisch.lua"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "Lyth Hub",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/Lythicals/script/main/Fisch.lua",true))()
   end, 
})

local mainTab = Window:CreateTab("가강전", nil) -- Title, Image
local mainSection = mainTab:CreateSection("가강전")

local Button = mainTab:CreateButton({
   Name = "나한테 슬로우-간지전용",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/Reapvitalized/TSB/refs/heads/main/ARCAURA.lua"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "진격의거인",
   Callback = function()
   loadstring(game:HttpGet("https://paste.ee/r/fxY03"))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "사타전용스크",
   Callback = function()
   loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Mahitotsbupdate'))()
   end, 
})

local mainTab = Window:CreateTab("펫시뮬", nil) -- Title, Image
local mainSection = mainTab:CreateSection("펫시뮬")

local Button = mainTab:CreateButton({
   Name = "허브1",
   Callback = function()
   loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Mahitotsbupdate'))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "허브2",
   Callback = function()
   loadstring(game:HttpGet("https://pastebin.com/raw/E7cx9p5m"))()
   end, 
})

local mainTab = Window:CreateTab("한국머더", nil) -- Title, Image
local mainSection = mainTab:CreateSection("한국머더")

local Button = mainTab:CreateButton({
   Name = "esp",
   Callback = function()
   loadstring(game:HttpGet('https://raw.githubusercontent.com/minute124/RH-666-/refs/heads/main/ee454504248d2435.lua'))()
   end, 
})

local mainTab = Window:CreateTab("좀비어택", nil) -- Title, Image
local mainSection = mainTab:CreateSection("좀비어택")

local Button = mainTab:CreateButton({
   Name = "허브",
   Callback = function()
   loadstring(game:HttpGet("https://bonkhubloader.netlify.app",true))()
   end, 
})

local mainTab = Window:CreateTab("보물섬만들기", nil) -- Title, Image
local mainSection = mainTab:CreateSection("보물섬만들기")

local Button = mainTab:CreateButton({
   Name = "허브1",
   Callback = function()
   loadstring(game:HttpGet("https://bonkhubloader.netlify.app",true))()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "허브2",
   Callback = function()
   loadstring(game:HttpGet"https://raw.githubusercontent.com/SkibidiCen/MainMenu/main/Code")()
   end, 
})

local Button = mainTab:CreateButton({
   Name = "오토팜",
   Callback = function()
   loadstring(game:HttpGet("https://raw.githubusercontent.com/ExyXyz/ExyGantenk/main/ExyBABFT"))()
   end, 
})
