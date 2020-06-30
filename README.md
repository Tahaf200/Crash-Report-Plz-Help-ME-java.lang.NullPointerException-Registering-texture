s# Crash-Report-Plz-Help-ME-java.lang.NullPointerException-Registering-texture
Plz help me and tell me what do i am very new to this 
the crash report:
---- Minecraft Crash Report ----
// There are four lights!

Time: 6/30/20 4:19 PM
Description: Registering texture

java.lang.NullPointerException: Registering texture
	at net.minecraft.client.resources.SimpleReloadableResourceManager.func_110536_a(SimpleReloadableResourceManager.java:63)
	at net.minecraft.client.renderer.texture.SimpleTexture.func_110551_a(SourceFile:29)
	at net.minecraft.client.renderer.texture.TextureManager.func_110579_a(TextureManager.java:89)
	at net.minecraft.client.renderer.texture.TextureManager.func_110577_a(TextureManager.java:45)
	at net.minecraft.client.gui.GuiMainMenu.func_73968_a(GuiMainMenu.java:400)
	at net.minecraft.client.gui.GuiMainMenu.func_73971_c(GuiMainMenu.java:434)
	at net.minecraft.client.gui.GuiMainMenu.func_73863_a(GuiMainMenu.java:461)
	at net.minecraft.client.renderer.EntityRenderer.func_78480_b(EntityRenderer.java:1061)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:1001)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:898)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at net.minecraft.client.resources.SimpleReloadableResourceManager.func_110536_a(SimpleReloadableResourceManager.java:63)
	at net.minecraft.client.renderer.texture.SimpleTexture.func_110551_a(SourceFile:29)
	at net.minecraft.client.renderer.texture.TextureManager.func_110579_a(TextureManager.java:89)

-- Resource location being registered --
Details:
	Resource location: ~~NULL~~
	Texture object class: net.minecraft.client.renderer.texture.SimpleTexture
Stacktrace:
	at net.minecraft.client.renderer.texture.TextureManager.func_110577_a(TextureManager.java:45)
	at net.minecraft.client.gui.GuiMainMenu.func_73968_a(GuiMainMenu.java:400)
	at net.minecraft.client.gui.GuiMainMenu.func_73971_c(GuiMainMenu.java:434)
	at net.minecraft.client.gui.GuiMainMenu.func_73863_a(GuiMainMenu.java:461)
	at net.minecraft.client.renderer.EntityRenderer.func_78480_b(EntityRenderer.java:1061)

-- Screen render details --
Details:
	Screen name: net.minecraft.client.gui.GuiMainMenu
	Mouse location: Scaled: (251, 268). Absolute: (502, 230)
	Screen size: Scaled: (512, 384). Absolute: (1024, 768). Scale factor of 2
Stacktrace:
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:1001)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:898)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 1362394688 bytes (1299 MB) / 6458703872 bytes (6159 MB) up to 11453595648 bytes (10923 MB)
	JVM Flags: 4 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx12288m -Xms256m -XX:PermSize=256m
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP v9.05 FML v7.10.99.99 Minecraft Forge 10.13.4.1614 457 mods loaded, 451 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UCHIJA	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) 
	UCHIJA	FML{7.10.99.99} [Forge Mod Loader] (forge-1.7.10-10.13.4.1614-1.7.10.jar) 
	UCHIJA	Forge{10.13.4.1614} [Minecraft Forge] (forge-1.7.10-10.13.4.1614-1.7.10.jar) 
	UCHIJA	da3dsoulASMFix{0.1.0} [DA3DSOUL ASM Fixes] (minecraft.jar) 
	UCHIJA	AM2-Preloader{0.0.3} [AMCore] (minecraft.jar) 
	UCHIJA	appliedenergistics2-core{rv3-beta-6} [Applied Energistics 2 Core] (minecraft.jar) 
	UCHIJA	Aroma1997Core{1.0.2.16} [Aroma1997Core] (Aroma1997Core-1.7.10-1.0.2.16.jar) 
	UCHIJA	BRCore{1.0} [BRCore] (minecraft.jar) 
	UCHIJA	CodeChickenCore{1.0.7.47} [CodeChicken Core] (minecraft.jar) 
	UCHIJA	ExtraFixes{1.2.4b} [Extra Fixes] (minecraft.jar) 
	UCHIJA	ImmibisMicroblocks{59.1.1} [Immibis's Microblocks] (immibis-microblocks-59.1.1.jar) 
	UCHIJA	InfiniBows{1.3.0 build 20} [InfiniBows] (minecraft.jar) 
	UCHIJA	ivtoolkit{1.2.1} [IvToolkit] (minecraft.jar) 
	UCHIJA	LambdaLib|Core{1.2.3} [LambdaLib|Core] (minecraft.jar) 
	UCHIJA	Micdoodlecore{} [Micdoodle8 Core] (minecraft.jar) 
	UCHIJA	NotEnoughItems{1.0.5.120} [Not Enough Items] (NotEnoughItems-1.7.10-1.0.5.120-universal.jar) 
	UCHIJA	OpenComputers|Core{1.7.4.1265} [OpenComputers (Core)] (minecraft.jar) 
	UCHIJA	PotionExtensionCore{1.7.10-1.1.0} [PotionExtensionCore] (minecraft.jar) 
	UCHIJA	RenderPlayerAPI{1.4} [Render Player API] (minecraft.jar) 
	UCHIJA	se{0.4.1} [Super Enchants] (minecraft.jar) 
	UCHIJA	technomCore{0.12.5} [Technomancy Core] (minecraft.jar) 
	UCHIJA	ThE-core{1.0.0.1} [Thaumic Energistics Core] (minecraft.jar) 
	UCHIJA	ThaumicTinkerer-preloader{0.1} [Thaumic Tinkerer Core] (minecraft.jar) 
	UCHIJA	voltzenginepreloader{0.0.1} [Voltz Engine Preloader] (minecraft.jar) 
	UCHIJA	WitchingGadgetsCore{1.1.10} [Witching Gadgets Core] (minecraft.jar) 
	UCHIJA	OpenModsCore{0.10} [OpenModsCore] (minecraft.jar) 
	UCHIJA	<CoFH ASM>{000} [CoFH ASM] (minecraft.jar) 
	UCHIJA	mod_ThreadedLighting{1.7.10-1.0} [Threaded Lighting] (minecraft.jar) 
	UCHIJA	targoss-mattock-direslime-fix{1.0.0} [Mattock DireSlime Fix] (minecraft.jar) 
	UCHIJA	FastCraft{1.25} [FastCraft] (fastcraft-1.25.jar) 
	UCHIJA	debug{1.0} [debug] (denseores-1.6.2.jar) 
	UCHIJA	gilded-games-util{1.7.10-1.2} [Gilded Games Utility] (Gilded-Games-Util-1.7.10.jar) 
	UCHIJA	ItemBlacklist{1.2.0.8} [ItemBlacklist] (ItemBlacklist-1.7.10-1.2.0.8.jar) 
	UCHIJA	Ambience{GRADLE:VERSION-GRADLE:BUILD} [Ambience] ((client)Ambience+1.0-3.jar) 
	UCHIJA	defaultkeys{1.0.28} [Default Keyconfig] ((client)defaultkeys-mc1.7.10-1.0.28.jar) 
	UCHIJA	notenoughkeys{@MOD_VERSION@} [NotEnoughKeys] ((client)NotEnoughKeys-1.7.10-3.0.0b45-dev-universal.jar) 
	UCHIJA	bt{1.0.2} [NotEnoughThaumcraftTabs] ((client)NotEnoughThaumcraftTabs-1.0.2.jar) 
	UCHIJA	reauth{3.5.0} [ReAuth] ((client)ReAuth-3.5.0.jar) 
	UCHIJA	ResourceLoader{1.3} [Resource Loader] ((client)ResourceLoader-MC1.7.10-1.3.jar) 
	UCHIJA	nevermine{Tslat-1.1.3} [Advent of Ascension] (AoA-Tslat-1.1.3.jar) 
	UCHIJA	appliedenergistics2{rv3-beta-6} [Applied Energistics 2] (appliedenergistics2-rv3-beta-6.jar) 
	UCHIJA	CoFHCore{1.7.10R3.1.4} [CoFH Core] (CoFHCore-[1.7.10]3.1.4-329.jar) 
	UCHIJA	Baubles{1.0.1.10} [Baubles] (Baubles-1.7.10-1.0.1.10.jar) 
	UCHIJA	ThermalFoundation{1.7.10R1.2.6} [Thermal Foundation] (ThermalFoundation-[1.7.10]1.2.6-118.jar) 
	UCHIJA	Mantle{1.7.10-0.3.2.jenkins191} [Mantle] (Mantle-1.7.10-0.3.2b.jar) 
	UCHIJA	thermaltinkering{1.0} [Thermal Tinkering] (ThermalTinkering-1.7.10-1.2.1.jar) 
	UCHIJA	ThermalExpansion{1.7.10R4.1.5} [Thermal Expansion] (ThermalExpansion-[1.7.10]4.1.5-248.jar) 
	UCHIJA	BigReactors{0.4.3A} [Big Reactors] (BigReactors-0.4.3A.jar) 
	UCHIJA	ForgeMultipart{1.2.0.347} [Forge Multipart] (ForgeMultipart-1.7.10-1.2.0.347-universal.jar) 
	UCHIJA	BuildCraft|Core{7.1.23} [BuildCraft] (buildcraft-7.1.23.jar) 
	UCHIJA	ExtraUtilities{1.2.12} [Extra Utilities] (extrautilities-1.2.12.jar) 
	UCHIJA	Thaumcraft{4.2.3.5} [Thaumcraft] (Thaumcraft-1.7.10-4.2.3.5.jar) 
	UCHIJA	Botania{r1.8-249} [Botania] (Botania r1.8-249.jar) 
	UCHIJA	MetallurgyCore{4.0.4} [Metallurgy Core] (MetallurgyCore-1.7.10-4.0.4.18.jar) 
	UCHIJA	AWWayofTime{v1.3.3} [Blood Magic: Alchemical Wizardry] (BloodMagic-1.7.10-1.3.3-17.jar) 
	UCHIJA	Avaritia{1.13} [Avaritia] (Avaritia-1.13.jar) 
	UCHIJA	IC2{2.2.827-experimental} [IndustrialCraft 2] (industrialcraft-2-2.2.827-experimental.jar) 
	UCHIJA	Railcraft{9.12.2.0} [Railcraft] (Railcraft_1.7.10-9.12.2.0.jar) 
	UCHIJA	ImmersiveEngineering{0.7.7} [Immersive Engineering] (ImmersiveEngineering-0.7.7.jar) 
	UCHIJA	MineFactoryReloaded{1.7.10R2.8.1} [MineFactory Reloaded] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	ComputerCraft{1.75} [ComputerCraft] (ComputerCraft1.75.jar) 
	UCHIJA	tc{4.4.1_020} [Traincraft] (Traincraft-4.4.1_020.jar) 
	UCHIJA	Waila{1.5.10} [Waila] (Waila-1.5.10_1.7.10.jar) 
	UCHIJA	TConstruct{1.7.10-1.8.8.build991} [Tinkers' Construct] (TConstruct-1.7.10-1.8.8.build991.jar) 
	UCHIJA	Metallurgy{4.0.6} [Metallurgy 4] (Metallurgy-1.7.10-4.0.6.80.jar) 
	UCHIJA	Natura{2.2.0} [Natura] (natura-1.7.10-2.2.1a2.jar) 
	UCHIJA	harvestcraft{1.7.10j} [Pam's HarvestCraft] (Pam_s HarvestCraft 1.7.10Lb.jar) 
	UCHIJA	progressiveautomation{1.6.35} [Progressive Automation] (ProgressiveAutomation-1.7.10-1.6.35.jar) 
	UCHIJA	cookiecore{1.4.0} [Cookie Core] (CookieCore-1.7.10-1.4.0-11.jar) 
	UCHIJA	MineTweaker3{3.0.10} [MineTweaker 3] (MineTweaker3-1.7.10-3.0.10B.jar) 
	UCHIJA	TSteelworks{1.7.10-1.1.2} [Tinkers' Steelworks] (TSteelworks-1.7.10-1.1.2-20.jar) 
	UCHIJA	ExtraTiC{1.4.6} [ExtraTiC] (ExtraTiC-1.7.10-1.4.6.jar) 
	UCHIJA	WailaHarvestability{1.1.6} [Waila Harvestability] ((client)WailaHarvestability-mc1.7.10-1.1.6.jar) 
	UCHIJA	wawla{1.3.1} [What Are We Looking At] ((client)Wawla-1.0.5.120.jar) 
	UCHIJA	securitycraft{v1.8.12} [SecurityCraft] ([1.7.10] SecurityCraft v1.8.12.jar) 
	UCHIJA	BuildCraft|Transport{7.1.23} [BC Transport] (buildcraft-7.1.23.jar) 
	UCHIJA	BuildCraft|Factory{7.1.23} [BC Factory] (buildcraft-7.1.23.jar) 
	UCHIJA	BuildCraft|Silicon{7.1.23} [BC Silicon] (buildcraft-7.1.23.jar) 
	UCHIJA	BuildCraft|Robotics{7.1.23} [BC Robotics] (buildcraft-7.1.23.jar) 
	UCHIJA	BuildCraft|Energy{7.1.23} [BC Energy] (buildcraft-7.1.23.jar) 
	UCHIJA	BuildCraft|Builders{7.1.23} [BC Builders] (buildcraft-7.1.23.jar) 
	UCHIJA	Additional-Buildcraft-Objects{MC1.7.10-BC7.1release4.0.10} [Additional Buildcraft Objects] (ABO-MC1.7.10-BC7.1release4.0.10.jar) 
	UCHIJA	abyssalcraft{1.9.1.3} [AbyssalCraft] (AbyssalCraft-1.7.10-1.9.1.3-FINAL.jar) 
	UCHIJA	LambdaLib{1.2.3} [LambdaLib] (LambdaLib-1.2.3.jar) 
	UCHIJA	academy-craft{1.0.7} [Academy Craft] (AcademyCraft-1.0.7.jar) 
	UCHIJA	AgriCraft{1.7.10-1.5.0} [AgriCraft] (AgriCraft-1.7.10-1.5.0.jar) 
	UCHIJA	mobdropcrops{1.7.2a} [Pam's Mob Drop Crops] (Pam_s+Mob+Drop+Crops+1.7.10a.zip) 
	UCHIJA	acmobdrops{0.11} [AgriCraft Mob Drop Crops] (ACMobDrops-1.7.10-0.11.jar) 
	UCHIJA	ActuallyAdditions{1.7.10-r21} [Actually Additions] (ActuallyAdditions-1.7.10-r21.jar) 
	UCHIJA	GalacticraftCore{3.0.12} [Galacticraft Core] (GalacticraftCore-1.7-3.0.12.504.jar) 
	UCHIJA	Mekanism{9.1.1} [Mekanism] (Mekanism-1.7.10-9.1.1.1031.jar) 
	UCHIJA	magicalcrops{4.0.0_PUBLIC_BETA_4b} [Magical Crops: Core] (magicalcrops-4.0.0_PUBLIC_BETA_5.jar) 
	UCHIJA	additionalrecipes{1.1} [Additional Recipes] (additionalrecipes-1.5.jar) 
	UCHIJA	bdlib{1.9.4.109} [BD Lib] (bdlib-1.9.4.109-mc1.7.10.jar) 
	UCHIJA	ae2stuff{0.5.1.9} [AE2 Stuff] (ae2stuff-rv3-0.5.1.9-mc1.7.10.jar) 
	UCHIJA	aether{1.7.10-1.6} [Aether II] (Aether-2-1.7.10.jar) 
	UCHIJA	AFSU{1.2.3a-Freeza} [AFSU Mod] (AFSU-1.2.3a-Freeza.jar) 
	UCHIJA	aiimprovements{0.0.1.19} [AI Improvements] (AIImprovements-1.7.10-0.0.1b19-dev.jar) 
	UCHIJA	AnimationAPI{1.2.4} [AnimationAPI] (AnimationAPI-1.7.10-1.2.4.jar) 
	UCHIJA	arsmagica2{1.4.0.009} [Ars Magica 2] (AM2-1.4.0.009.jar) 
	UCHIJA	AncientWarfare{2.4.114-beta-MC1.7.10} [Ancient Warfare Core] (ancientwarfare-2.4.115-beta-MC1.7.10-FULL.jar) 
	UCHIJA	AncientWarfareAutomation{2.4.114-beta-MC1.7.10} [Ancient Warfare Automation] (ancientwarfare-2.4.115-beta-MC1.7.10-FULL.jar) 
	UCHIJA	AncientWarfareNEIPlugin{2.4.114-beta-MC1.7.10} [Ancient Warfare NEI Plugin] (ancientwarfare-2.4.115-beta-MC1.7.10-FULL.jar) 
	UCHIJA	AncientWarfareNpc{2.4.114-beta-MC1.7.10} [Ancient Warfare NPCs] (ancientwarfare-2.4.115-beta-MC1.7.10-FULL.jar) 
	UCHIJA	AncientWarfareStructure{2.4.114-beta-MC1.7.10} [Ancient Warfare Structures] (ancientwarfare-2.4.115-beta-MC1.7.10-FULL.jar) 
	UCHIJA	aobdsingularities{1.0.4} [Another One Bites The Dust: Singularities] (AOBDsingularities-1.0.4.jar) 
	UCHIJA	AppleCore{3.1.1} [AppleCore] (AppleCore-mc1.7.10-3.1.1.jar) 
	UCHIJA	arcane_engineering{0.2.7} [Arcane Engineering] (arcane_engineering-0.2.7.jar) 
	UCHIJA	arcanearteries{5} [Arcane Arteries] (ArcaneArteries0.8.2.jar) 
	UCHIJA	MovingWorld{1.7.10-1.8.1} [Moving World] (movingworld-1.7.10-1.8.1.jar) 
	UCHIJA	ArchimedesShipsPlus{1.7.10-1.8.1} [Archimedes' Ships Plus] (archimedesshipsplus-1.7.10-1.8.1.jar) 
	UCHIJA	ArchitectureCraft{1.7.2} [ArchitectureCraft] (ArchitectureCraft-1.7.2-mc1.7.10.jar) 
	UCHIJA	Aroma1997CoreHelper{1.0.2.16} [Aroma1997Core|Helper] (Aroma1997Core-1.7.10-1.0.2.16.jar) 
	UCHIJA	Aroma1997sDimension{1.0} [Aroma1997's Dimensional World] (Aroma1997s-Dimensional-World-1.7.10-1.1.0.1.jar) 
	UCHIJA	AromaBackup{0.1.0.0} [AromaBackup] (AromaBackup-1.7.10-0.1.0.0.jar) 
	UCHIJA	AromaBackupRecovery{1.0} [AromaBackup Recovery] (AromaBackup-1.7.10-0.1.0.0.jar) 
	UCHIJA	aura{unspecified} [Aura Cascade] (AuraCascade-557.jar) 
	UCHIJA	MineFactoryReloaded|CompatThaumcraft{1.7.10R2.8.1} [MFR Compat: Thaumcraft] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	Automagy{0.28.2} [Automagy] (Automagy-1.7.10-0.28.2.jar) 
	UCHIJA	AutomatedRedstone{2.1.0} [Automated Redstone] (AutomatedRedstone-1.7.10-2.2.1.jar) 
	UCHIJA	autopackager{1.5.9a} [AutoPackager] (autopackager-1.5.9a.jar) 
	UCHIJA	wanionlib{1.7.10-1.8} [WanionLib] (WanionLib-1.7.10-1.8.jar) 
	UCHIJA	avaritiaddons{1.4b} [Avaritiaddons] (Avaritiaddons-1.4b.jar) 
	UCHIJA	Backpack{2.0.1} [Backpack] (backpack-2.0.1-1.7.x.jar) 
	UCHIJA	BetterAchievements{0.1.0} [Better Achievements] (BetterAchievements-1.7.10-0.1.0.jar) 
	UCHIJA	betterbuilderswands{0.8.1} [Better Builder's Wands] (BetterBuildersWands-0.8.1-1.7.10r92+aec06c3.jar) 
	UCHIJA	BetterChests{1.1.1.9} [BetterChests] (BetterChests-1.7.10-1.1.1.9.jar) 
	UCHIJA	betterquesting{2.0.233} [Better Questing] (BetterQuesting-2.0.233.jar) 
	UCHIJA	BiblioCraft{1.11.7} [BiblioCraft] (BiblioCraft[v1.11.7][MC1.7.10].jar) 
	UCHIJA	HardcoreEnderExpansion{1.8.6} [Hardcore Ender Expansion] (HardcoreEnderExpansion  MC-1.7.10  v1.8.6.jar) 
	UCHIJA	Forestry{4.2.16.64} [Forestry for Minecraft] (forestry_1.7.10-4.2.16.64.jar) 
	UCHIJA	BinnieCore{2.0.22.7} [Binnie Core] (binnie-mods-1.7.10-2.0.22.7.jar) 
	UCHIJA	Botany{2.0.22.7} [Botany] (binnie-mods-1.7.10-2.0.22.7.jar) 
	UCHIJA	ExtraTrees{2.0.22.7} [Extra Trees] (binnie-mods-1.7.10-2.0.22.7.jar) 
	UCHIJA	Genetics{2.0.22.7} [Genetics] (binnie-mods-1.7.10-2.0.22.7.jar) 
	UCHIJA	ExtraBees{2.0.22.7} [Extra Bees] (binnie-mods-1.7.10-2.0.22.7.jar) 
	UCHIJA	BioCristals{1.8.11} [Bio Cristals] (BioCristals-1.7.10-1.8.11.jar) 
	UCHIJA	BlockProperties{0.1.5} [Block Properties] (BlockProperties-1.7.10-0.1.5.jar) 
	UCHIJA	ThaumicTinkerer{unspecified} [Thaumic Tinkerer] (ThaumicTinkerer-2.5-1.7.10-164.jar) 
	UCHIJA	ForbiddenMagic{1.7.10-0.575} [Forbidden Magic] (Forbidden Magic-1.7.10-0.575.jar) 
	UCHIJA	guideapi{1.7.10-1.0.1-29} [Guide-API] (Guide-API-1.7.10-1.0.1-29.jar) 
	UCHIJA	BloodArsenal{1.2-5} [Blood Arsenal] (BloodArsenal-1.7.10-1.2-5.jar) 
	UCHIJA	boilerplate{6.3.0.81} [Boilerplate] (boilerplate-1.7.10-6.3.0.81-universal.jar) 
	UCHIJA	bookshelf{1.0.4.187} [Bookshelf] (Bookshelf-1.7.10-1.0.4.187.jar) 
	UCHIJA	BrandonsCore{1.0.0.12} [Brandon's Core] (BrandonsCore-1.0.0.12.jar) 
	UCHIJA	BuildCraft|Compat{7.1.7} [BuildCraft Compat] (buildcraft-compat-7.1.7.jar) 
	UCHIJA	eureka{3.0.2} [Eureka] (Eureka-1.7.10-3.0.2.jar) 
	UCHIJA	bcadditions{2.2.5} [BuildCraft Additions] (BuildcraftAdditions-1.7.10-2.2.5.jar) 
	UCHIJA	buildersguides{1.7.10-1.0.2} [Builder's Guides] (buildersguides-1.7.10-1.0.2.jar) 
	UCHIJA	SonarCore{1.1.3} [SonarCore] (SonarCore-1.7.10-1.1.3.jar) 
	UCHIJA	Calculator{1.9.11} [Calculator] (Calculator-1.7.10-1.9.11.jar) 
	UCHIJA	CalendarAPI{@VERSION@} [CalendarAPI] (Calendar-1.7.10-1.0-4.jar) 
	UCHIJA	TwilightForest{2.3.8dev} [The Twilight Forest] (twilightforest-1.7.10-2.3.8dev-clienthax.jar) 
	UCHIJA	chisel{2.9.5.11} [Chisel] (Chisel-2.9.5.11.jar) 
	UCHIJA	CarpentersBlocks{3.3.8.1} [Carpenter's Blocks] (Carpenter_s Blocks v3.3.8.1 - MC 1.7.10.jar) 
	UCHIJA	catwalks{2.0.4} [Catwalks Mod] (catwalks-2.0.4.jar) 
	UCHIJA	catwalkmod{x.x.x} [Legacy Catwalk Compat] (catwalks-2.0.4.jar) 
	UCHIJA	ChestTransporter{2.0.6} [Chest Transporter] (ChestTransporter-1.7.10-2.0.6.jar) 
	UCHIJA	ChiselFacades{1.7.10-2.12-chiselteam} [Chisel Facades] (ChiselFacades-1.7.10-2.12-chiselteam.jar) 
	UCHIJA	Ztones{1.7.10} [Ztones] (Ztones-1.7.10-2.2.1.jar) 
	UCHIJA	chiseltones{@VERSION@} [Chisel Tones] (ChiselTones-1.7.10-1.0-3.jar) 
	UCHIJA	CLG{2.0.1} [Compact Lava Generator] (CLG-2.0.1.jar) 
	UCHIJA	compacter{1.1.0.12} [Compacter] (compacter-1.1.0.12-mc1.7.10.jar) 
	UCHIJA	EnderStorage{1.4.7.37} [EnderStorage] (EnderStorage-1.7.10-1.4.7.37-universal.jar) 
	UCHIJA	MrTJPCoreMod{1.1.0.33} [MrTJPCore] (MrTJPCore-1.7.10-1.1.0.33-universal.jar) 
	UCHIJA	ProjRed|Core{4.7.0pre12.95} [ProjectRed Core] (ProjectRed-1.7.10-4.7.0pre12.95-Base.jar) 
	UCHIJA	ProjRed|Transmission{4.7.0pre12.95} [ProjectRed Transmission] (ProjectRed-1.7.10-4.7.0pre12.95-Integration.jar) 
	UCHIJA	OpenComputers{1.7.4.1265} [OpenComputers] (OpenComputers-MC1.7.10-1.7.4.1265-universal.jar) 
	UCHIJA	PneumaticCraft{1.12.7-152} [PneumaticCraft] (PneumaticCraft-1.7.10-1.12.7-152-universal.jar) 
	UCHIJA	CompactMachines{1.7.10-1.21} [Compact Machines] (compactmachines-1.7.10-1.21.jar) 
	UCHIJA	CompactSolars{4.4.39.315} [Compact Solar Arrays] (CompactSolars-1.7.10-4.4.39.315-universal.jar) 
	UCHIJA	compactstorage{v2.0.0a} [CompactStorage] (compactstorage-1.7.10-release-2.1.0-lts.21-universal.jar) 
	UCHIJA	contraptions{0.1.5} [Contraptions] (Contraptions-1.7.10-0.1.5.jar) 
	UCHIJA	cookingbook{1.0.140} [Cooking for Blockheads] (cookingbook-mc1.7.10-1.0.140.jar) 
	UCHIJA	CoroAI{v1.0} [CoroAI] (coroutil-1.7.10-1.1.6.jar) 
	UCHIJA	BuildMod{v1.0} [Build Mod] (coroutil-1.7.10-1.1.6.jar) 
	UCHIJA	CoroPets{v1.0} [CoroPets] (coroutil-1.7.10-1.1.6.jar) 
	UCHIJA	ExtendedRenderer{v1.0} [Extended Renderer] (coroutil-1.7.10-1.1.6.jar) 
	UCHIJA	ConfigMod{v1.0} [Extended Mod Config] (coroutil-1.7.10-1.1.6.jar) 
	UCHIJA	craftarcanum{1.1.1} [Craft Arcanum] (CraftArcanum-1.1.1.jar) 
	UCHIJA	craftingcraft{1.0.12} [CraftingCraft] (craftingcraft-mc1.7.10-1.0.13.jar) 
	UCHIJA	craftingtweaks{1.0.88} [Crafting Tweaks] (craftingtweaks-mc1.7.10-1.0.88.jar) 
	UCHIJA	creativecore{1.3.14} [CreativeCore] (CreativeCore+v1.3.24+mc1.7.10.jar) 
	UCHIJA	CustomPets{1.0.5} [Custom Pets] (custompets-1.7.10-1.0.5-universal.jar) 
	UCHIJA	endercore{1.7.10-0.2.0.39_beta} [EnderCore] (EnderCore-1.7.10-0.2.0.39_beta.jar) 
	UCHIJA	customthings{MC1.7.10-0.0.3-55} [CustomThings] (CustomThings-MC1.7.10-0.0.3-55.jar) 
	UCHIJA	D3Core{1.1.2.41} [D3Core] (D3Core-1.7.10-1.1.2.41.jar) 
	UCHIJA	darkcore{0.3} [Dark Core] (darkcore-0.3-86.jar) 
	UCHIJA	PTRModelLib{1.0.0} [PTRModelLib] (Decocraft-2.4.2_1.7.10.jar) 
	UCHIJA	props{2.4.2} [Decocraft] (Decocraft-2.4.2_1.7.10.jar) 
	UCHIJA	DefenseTech{1.0.1} [DefenseTech] (DefenseTech-1.7.10-1.0.1.46.jar) 
	UCHIJA	DimensionalCore{1.0.7} [DimensionalCore] (DimensionalCore-1.7.10-1.0.7.jar) 
	UCHIJA	dmtweaks{1.0.0} [DMTweaks] (DMTweaks-1.0.0.jar) 
	UCHIJA	doggytalents{1.14.2.317} [Doggy Talents] (DoggyTalents-1.7.10-1.14.2.317-universal.jar) 
	UCHIJA	dldungeonsjdg{1.11.0.1} [Doomlike Dungeons] (DoomlikeDungeons-1.11.0.1-MC1.7.10.jar) 
	UCHIJA	DraconicEvolution{1.0.2h} [Draconic Evolution] (Draconic-Evolution-1.7.10-1.0.2h.jar) 
	UCHIJA	DragonsRadioMod{1.7.1} [Dragon's Radio Mod] (Dragon_s+Radio+Mod-MC1.7.10-1.7.1.jar) 
	UCHIJA	DummyCore{1.13} [DummyCore] (DummyCore1.13.jar) 
	UCHIJA	ea{v2.3.4c-mc1.7.10} [Ebon Arts] (EbonArts-v2.3.4c-mc1.7.10.jar) 
	UCHIJA	eiorteis{1.7.10-1.3} [EIORecipesTEInductionSmelter] (eiorteis-1.3.jar) 
	UCHIJA	eplus{4.0.0..73} [Enchanting Plus] (EnchantingPlus-1.7.10-4.0.0.74.jar) 
	UCHIJA	Enchiridion{1.3} [Enchiridion] (Enchiridion+2-1.7.10-2.0.2a.jar) 
	UCHIJA	Enchiridion2{2.0.2a} [Enchiridion 2] (Enchiridion+2-1.7.10-2.0.2a.jar) 
	UCHIJA	EnderIO{1.7.10-2.3.0.429_beta} [Ender IO] (EnderIO-1.7.10-2.3.0.429_beta.jar) 
	UCHIJA	waterhooks{1.2.1} [Water Hooks] (waterhooks-1.2.1.jar) 
	UCHIJA	enderioaddons{0.10.13} [Ender IO Addons] (EnderIOAddons-1.7.10-2.3.0.427_beta-0.10.13.56_beta.jar) 
	UCHIJA	EnderTech{1.7.10-0.3.2.405} [EnderTech] (EnderTech-1.7.10-0.3.2.405.jar) 
	UCHIJA	enderutilities{0.5.3} [Ender Utilities] (enderutilities-1.7.10-0.5.3.jar) 
	UCHIJA	eng_toolbox{1.2.3.0} [Engineer's Toolbox] (EngineersToolbox-1.2.3.0-BETA.jar) 
	UCHIJA	EnhancedArmors{1.7.10-1.0a MorelPlay} [EnhancedArmors] (Enhanced Armors 1.7.10-1.0 MorelPlay.jar) 
	UCHIJA	enhancedportals{3.0.12} [EnhancedPortals] (EnhancedPortals_1.7.10-universal-3.0.12.jar) 
	UCHIJA	EntityBlocker{1.1.0MC1.7.10} [EntityBlocker] (EntityBlocker-1.7.10-1.1.jar) 
	UCHIJA	ProjectE{1.7.10-PE1.10.1} [ProjectE] (ProjectE-1.7.10-PE1.10.1.jar) 
	UCHIJA	equivalentenergistics{0.8.3} [Equivalent Energistics] (EquivalentEnergistics-1.7.10-0.8.3.jar) 
	UCHIJA	thermsingul{1.7.10-1.2} [Thermal Singularities] (ThermalSingularities-1.7.10-1.2.jar) 
	UCHIJA	universalsingularities{1.7.10-8.0} [Universal Singularities] (Universal Singularities [Version 8]-1.7.10.jar) 
	UCHIJA	eternalsingularity{1.7.10-.1.0.4b} [Eternal Singularity] (EternalSingularity-1.7.10-1.0.4b.jar) 
	UCHIJA	evilcraft{0.9.13} [EvilCraft] (EvilCraft-1.7.10-0.9.13.jar) 
	UCHIJA	ewysworkshop{Ewy's Workshop-1.7.10-1.1.5} [Ewy's Workshop] (Ewy_s Workshop-1.1.6.jar) 
	UCHIJA	ExpandedIndustry{15.26.1a} [Expanded Industry] (ExpandedIndustry-15.26.1a.jar) 
	UCHIJA	golems{1.20} [Extra Golems] (Extra-Golems[1.7.10]-1.20.jar) 
	UCHIJA	extracells{2.3.14} [Extra Cells 2] (ExtraCells-1.7.10-2.3.14b200.jar) 
	UCHIJA	extracoal{1.0.2} [Extra Coal] (Extracoal-1.7.10-1.0.2.jar) 
	UCHIJA	golems_addon_metals{1.12} [Metal Golems Addon] (ExtraGolemsMetalAddon[1.7.10]-1.12.jar) 
	UCHIJA	golems_addon_tconstruct{1.08} [Tinkers' Golems Addon] (ExtraGolemsTinkersAddon[1.7.10]-1.08.jar) 
	UCHIJA	golems_addon_waila{1.07} [Extra Golems Waila Addon] (ExtraGolemsWailaAddon[1.7.10]-1.07.jar) 
	UCHIJA	ezstorage{1.1.0} [EZ Storage] (ezstorage-1.1.0.jar) 
	UCHIJA	fluxedtrinkets{0.54} [Fluxed Trinkets] (Fluxed Trinkets-1.7.10-1.0.54.jar) 
	UCHIJA	llibrary{1.5.1} [LLibrary] (llibrary-1.5.1-1.7.10.jar) 
	UCHIJA	fossil{7.3.2} [Fossils and Archeology Revival] (fossilsarcheology-7.3.2.jar) 
	UCHIJA	FTBL{1.0.18.2} [FTBLib] (FTBLib-1.7.10-1.0.18.3.jar) 
	UCHIJA	FTBU{1.0.18.2} [FTBUtilities] (FTBUtilities-1.7.10-1.0.18.3.jar) 
	UCHIJA	furnus{1.75} [Furnus] (Furnus-1.7.10-1.75-final.jar) 
	UCHIJA	gadomancy{1.0.7.3} [Gadomancy] (gadomancy-1.7.10-1.0.7.3.jar) 
	UCHIJA	GalacticraftMars{3.0.12} [Galacticraft Planets] (Galacticraft-Planets-1.7-3.0.12.504.jar) 
	UCHIJA	RedstoneArsenal{1.7.10R1.1.2} [Redstone Arsenal] (RedstoneArsenal-[1.7.10]1.1.2-92.jar) 
	UCHIJA	MagicBees{2.4.4} [Magic Bees] (magicbees-1.7.10-2.4.4.jar) 
	UCHIJA	gendustry{1.6.3.132} [GenDustry] (gendustry-1.6.3.132-mc1.7.10.jar) 
	UCHIJA	pressure{1.3.0.fix1} [Pressure Pipes] (pressure-1.3.0.fix1-mc1.7.10.jar) 
	UCHIJA	advgenerators{0.9.20.123} [Advanced Generators] (generators-0.9.20.123-mc1.7.10.jar) 
	UCHIJA	getoffmytardis{1.0} [Get Off My Tardis] (getoffmytardis-1.1.jar) 
	UCHIJA	gvc{0.6.1} [§aGliby's§f Voice Chat Mod] (GlibysVC-1.7.10-0.6.2a.jar) 
	UCHIJA	GraviSuite{1.7.10-2.0.3} [Graviation Suite] (gravisuite-1.7.10-2.0.3.jar) 
	UCHIJA	iChunUtil{4.2.3} [iChunUtil] (iChunUtil-4.2.3.jar) 
	UCHIJA	GraviGun{4.0.0-beta} [GraviGun] (GravityGun-4.0.0-beta.jar) 
	UCHIJA	gud_thaumicnei{1.3.0} [Thaumic NEI] (gud_thaumicnei-1.3.0.jar) 
	UCHIJA	GunCus{1.7.10-3.51.0.-} [Gun Customization] (GunCustomization-1.7.10-3.51.0.-.jar) 
	UCHIJA	hammerz{0.1.7.37} [Hammerz] (Hammerz-1.7.10-0.1.7.37.jar) 
	UCHIJA	hardcorewither{1.1.3} [Hardcore Wither] (Hardcore Wither-1.7.10-1.1.3-21-universal.jar) 
	UCHIJA	hbm{1.0.27 BETA (3515)} [Hbm's Nuclear Tech] (hbm_1.0.27_X3515.jar) 
	UCHIJA	hgp{Release} [Horizontal Glass Panes] (hgp-1.7.10-1.1.0.4-universal.jar) 
	UCHIJA	HoloInventory{1.9.1.124} [HoloInventory] (HoloInventory-1.7.10-1.9.1.124.jar) 
	UCHIJA	HopperDuctMod{1.3.2} [Hopper Ducts] (hopperductmod-1.7.10-1.3.2.jar) 
	UCHIJA	IC2NuclearControl{2.4.3a} [Nuclear Control 2] (IC2NuclearControl-2.4.3a.jar) 
	UCHIJA	IGWMod{1.1.12-34} [In-Game wiki Mod] (IGW-Mod-1.7.10-1.1.12-34-universal.jar) 
	UCHIJA	immersiveintegration{0.6.8} [Immersive Integration] (immersiveintegration-0.6.8.jar) 
	UCHIJA	ImmibisCore{59.1.4} [Immibis Core] (immibis-core-59.1.4.jar) 
	UCHIJA	ImmibisPeripherals{59.0.3} [Immibis's Peripherals] (immibis-peripherals-59.0.3.jar) 
	UCHIJA	IndustrialExpansion{BETA-v1.1.2-var1} [Industrial Expansion] (IndustrialExpansion-BETA-v1.1.2-var1.jar) 
	UCHIJA	inpure|core{1.7.10R1.0.0B9} [INpureCore] (INpureCore-[1.7.10]1.0.0B9-62.jar) 
	UCHIJA	intellie{2.2.1.610} [IntelliE] (IntelligentEnergistics-1.7.10-2.2.1.610-universal.jar) 
	UCHIJA	appaero{2.2.1.610} [AppliedAerodynamics] (IntelligentEnergistics-1.7.10-2.2.1.610-universal.jar) 
	UCHIJA	appaeronei{2.2.1.610} [AppliedAerodynamicsNEI] (IntelligentEnergistics-1.7.10-2.2.1.610-universal.jar) 
	UCHIJA	appint{${version}} [AppliedIntelligences] (IntelligentEnergistics-1.7.10-2.2.1.610-universal.jar) 
	UCHIJA	InventoryPets{1.5.2} [Inventory Pets] (inventorypets-1.7.10-1.5.2-universal.jar) 
	UCHIJA	inventorytweaks{1.59-dev-152-cf6e263} [Inventory Tweaks] (InventoryTweaks-1.59-dev-152.jar) 
	UCHIJA	ironbackpacks{1.7.10-1.2.20} [Iron Backpacks] (IronBackpacks-1.7.10-1.2.20.jar) 
	UCHIJA	IronChest{6.0.62.742} [Iron Chest] (ironchest-1.7.10-6.0.62.742-universal.jar) 
	UCHIJA	ironfurnaces{1.2.4} [Iron Furnaces] (ironfurnaces-1.2.4R.jar) 
	UCHIJA	irontank{1.7.10-1.1.16.16} [Iron Tanks] (irontanks-1.7.10-1.1.16.16.jar) 
	UCHIJA	journeymap{5.1.4p2} [JourneyMap] (journeymap-1.7.10-5.1.4p2-unlimited.jar) 
	UCHIJA	jurassicraft{1.5.0} [JurassiCraft] (JurassiCraft-1.4.0.jar) 
	UCHIJA	je_calculation{0.3.4} [Just Enough Calculation] (JustEnoughCalculation-1.7.10-0.3.4.jar) 
	UCHIJA	koresample{1.7.10-1.3.2} [Kore Sample] (KoreSample-1.7.10-1.3.2.jar) 
	UCHIJA	lightningcraft{1.5.0} [LightningCraft] (LightningCraft-1.5.0-[1.7.10].jar) 
	UCHIJA	LightTweaks{0.21} [Lightwave's Tweaks] (LightTweaks-0.21.jar) 
	UCHIJA	LogisticsPipes{0.9.3.132} [Logistics Pipes] (logisticspipes-0.9.3.132.jar) 
	UCHIJA	LunatriusCore{1.1.2.21} [LunatriusCore] (LunatriusCore-1.7.10-1.1.2.21-universal.jar) 
	UCHIJA	magicalcropsarmour{4.0.0_PUBLIC_BETA_4} [Magical Crops: Armoury] (magicalcropsarmoury-4.0.0_PUBLIC_BETA_4.jar) 
	UCHIJA	magicalcropsdeco{4.0.0_PUBLIC_BETA_4a} [Magical Crops: Decorative] (magicalcropsdeco-4.0.0_PUBLIC_BETA_4a.jar) 
	UCHIJA	Magneticraft{0.6.0-final} [Magneticraft] (magneticraft-0.6.1-final.jar) 
	UCHIJA	magnanimoustools{1.0.8} [Magnanimous Tools] (MagTools-1.7.10-1.0.8.jar) 
	UCHIJA	malisiscore{1.7.10-0.14.3} [MalisisCore] (malisiscore-1.7.10-0.14.3.jar) 
	UCHIJA	malisisdoors{1.7.10-1.13.2} [Malisis' Doors] (malisisdoors-1.7.10-1.13.2.jar) 
	UCHIJA	mo{0.4.2} [Matter Overdrive] (MatterOverdrive-1.7.10-0.4.2.jar) 
	UCHIJA	RadixCore{2.1.3} [RadixCore] (RadixCore-1.7.10-2.1.3-universal.jar) 
	UCHIJA	MCA{1.7.10-5.2.2} [Minecraft Comes Alive] (MCA-1.7.10-5.2.2-universal.jar) 
	UCHIJA	MekanismGenerators{9.1.1} [MekanismGenerators] (MekanismGenerators-1.7.10-9.1.1.1031.jar) 
	UCHIJA	MekanismTools{9.1.1} [MekanismTools] (MekanismTools-1.7.10-9.1.1.1031.jar) 
	UCHIJA	metallurgychisel{1.0.0.11} [Metallurgy Chisel] (MetallurgyChisel-1.7.10-1.0.0.11.jar) 
	UCHIJA	metallurgycm{0.1.0} [Metallurgy Classic Machines] (MetallurgyClassicMachines-1.7.10-1.0.3.75.jar) 
	UCHIJA	voltzengine{1.11.0.491} [Voltz Engine] (VoltzEngine-1.7.10-1.11.0b491.jar) 
	UCHIJA	mffs{4.0.0.151} [Modular Forcefield System] (Mffs-1.7.10-4.0.0b151.jar) 
	UCHIJA	NetherOres{1.7.10R2.3.1} [Nether Ores] (NetherOres-[1.7.10]2.3.1-22.jar) 
	UCHIJA	Mimicry{1.7.x_1492_1.0.10} [Mimicry] (Mimicry-1.7.10_1492_1.0.10c.jar) 
	UCHIJA	MineFactoryReloaded|CompatAppliedEnergistics{1.7.10R2.8.1} [MFR Compat: Applied Energistics] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatBuildCraft{1.7.10R2.8.1} [MFR Compat: BuildCraft] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatForestry{1.7.10R2.8.1} [MFR Compat: Forestry] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatForgeMicroblock{1.7.10R2.8.1} [MFR Compat: ForgeMicroblock] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatIC2{1.7.10R2.8.1} [MFR Compat: IC2] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	ProjRed|Exploration{4.7.0pre12.95} [ProjectRed Exploration] (ProjectRed-1.7.10-4.7.0pre12.95-World.jar) 
	UCHIJA	MineFactoryReloaded|CompatProjRed{1.7.10R2.8.1} [MFR Compat ProjectRed] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatRailcraft{1.7.10R2.8.1} [MFR Compat: Railcraft] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatThermalExpansion{1.7.10R2.8.1} [MFR Compat: Thermal Expansion] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatTConstruct{1.7.10R2.8.1} [MFR Compat: Tinkers' Construct] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatTwilightForest{1.7.10R2.8.1} [MFR Compat: TwilightForest] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MineFactoryReloaded|CompatVanilla{1.7.10R2.8.1} [MFR Compat: Vanilla] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UCHIJA	MTRM{1.0} [MineTweakerRecipeMaker] (MineTweakerRecipeMaker-1.7.10-1.1.1.jar) 
	UCHIJA	mopickaxes{630} [Mo' Pickaxes] (Mo-Pickaxes-Mod-1.7.10.jar) 
	UCHIJA	moarcarts{1.2.4-null} [MoarCarts] (moarcarts-1.7.10-1.2.4-11.jar) 
	UCHIJA	modtweaker2{0.9.6} [Mod Tweaker 2] (ModTweaker2-0.9.6.jar) 
	UCHIJA	nhlib{2.0.11} [NHAVE's Library] (nhlib-1.7.10-2.0.11.jar) 
	UCHIJA	nhwrench{3.1.6} [NHAVE's OmniWrench V3] (nhwrench-1.7.10-3.1.6.jar) 
	UCHIJA	numina{1.7.10} [Numina] (Numina-0.4.1.106.jar) 
	UCHIJA	p455w0rdslib{1.0.4} [p455w0rd's Library] (p455w0rdslib-1.7.10-1.0.4.jar) 
	UCHIJA	ae2wct{1.7.10-rv3-1.8.7.9b} [AE2 Wireless Crafting Terminal] (WirelessCraftingTerminal-1.7.10-rv3-1.8.7.9b.jar) 
	UCHIJA	powersuits{1.7.10-0.11.1.117} [MachineMuse's Modular Powersuits] (ModularPowersuits-1.7.10-0.11.1.117.jar) 
	UCHIJA	MoreFurnaces{1.3.9} [More Furnaces] (MoreFurnaces-1.3.9-MC1.7.10.jar) 
	UCHIJA	moreShearables{1.0} [More Shearables] (MoreShearables1.0-1.7.10.jar) 
	UCHIJA	cfm{3.4.7} [§9MrCrayfish's Furniture Mod] (MrCrayfishFurnitureModv3.4.7(1.7.10).jar) 
	UCHIJA	MSM3{3.0.0d} [More Swords 3] (MSM-SNAP-3.0.0e-For-MC-1.7.10.jar) 
	UCHIJA	naturescompass{1.3.1} [Nature's Compass] (NaturesCompass-1.7.10-1.3.1.jar) 
	UCHIJA	NEIAddons{1.12.14.40} [NEI Addons] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJA	NEIAddons|Developer{1.12.14.40} [NEI Addons: Developer Tools] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJA	NEIAddons|AppEng{1.12.14.40} [NEI Addons: Applied Energistics 2] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJA	NEIAddons|Botany{1.12.14.40} [NEI Addons: Botany] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJA	NEIAddons|Forestry{1.12.14.40} [NEI Addons: Forestry] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJA	NEIAddons|CraftingTables{1.12.14.40} [NEI Addons: Crafting Tables] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJA	NEIAddons|ExNihilo{1.12.14.40} [NEI Addons: Ex Nihilo] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJA	nhintegration{1.0.12} [NHWRENCH Integrations] (nhintegration-1.7.10-1.0.12.jar) 
	UCHIJA	recipehandler{1.7.10} [NoMoreRecipeConflict] (NoMoreRecipeConflict-0.3(1.7.10).jar) 
	UCHIJA	notenoughIDs{1.4.3.4} [NotEnoughIDs] (NotEnoughIDs-1.4.3.4.jar) 
	UCHIJA	neresources{0.1.0.ManuallyBuilt} [Not Enough Resources] (NotEnoughResources-1.7.10-0.1.0-128.jar) 
	UCHIJA	NuclearCraft{1.9g} [NuclearCraft] (NuclearCraft-1.9g--1.7.10.jar) 
	UCHIJA	NVLIC2Machines{1.7.10.1558.1.1} [NVLIC2Machines] (NVLIC2Machines-1.7.10.1558.1.3.jar) 
	UCHIJA	NVLSimpleBlocks{1.7.10.1558.1.1} [NVLSimpleBlocks] (NVLSimpleBlocks-1.7.10.1558.1.1.jar) 
	UCHIJA	ocminecart{1.7} [OC-Minecarts] (ocminecart-1.7-oc1.5.jar) 
	UCHIJA	OpenMods{0.10} [OpenMods] (OpenModsLib-1.7.10-0.10.jar) 
	UCHIJA	OpenBlocks{1.6} [OpenBlocks] (OpenBlocks-1.7.10-1.6.jar) 
	UCHIJA	openmodularturrets{2.2.11-245} [Open Modular Turrets] (OpenModularTurrets-1.7.10-2.2.11-245.jar) 
	UCHIJA	OpenPeripheralCore{1.4} [OpenPeripheralCore] (OpenPeripheralCore-1.7.10-1.4.jar) 
	UCHIJA	OpenPeripheral{0.6} [OpenPeripheralAddons] (OpenPeripheralAddons-1.7.10-0.6.jar) 
	UCHIJA	OpenPeripheralIntegration{0.6} [OpenPeripheralIntegration] (OpenPeripheralIntegration-1.7.10-0.6.jar) 
	UCHIJA	openradio{0.6.1} [OpenRadio] (OpenRadio-0.6.1.jar) 
	UCHIJA	opensecurity{1.0.117} [OpenSecurity] (OpenSecurity-1.7.10-1.0-117.jar) 
	UCHIJA	fodc{1.6.1} [Ore Dictionary Converter] (OreDictionaryConverter-1.6.1.jar) 
	UCHIJA	OreSpawn{1.7.10.20.3} [OreSpawn] (orespawn-1.7.10-20.3.zip) 
	UCHIJA	origin{8.0.3} [Origin] (Origin-1.7.10-8.0.3.jar) 
	UCHIJA	addonscrewdriver{1.0.0} [OriginAddonScrewdriver] (Origin-1.7.10-8.0.3.jar) 
	UCHIJA	planetguyLib{1.9} [planetguyLib] (PlanetguyLib-1.9.2.jar) 
	UCHIJA	PortalGun{4.0.0-beta-6} [PortalGun] (PortalGun-4.0.0-beta-6-fix-1.jar) 
	UCHIJA	PowerConverters3{1.7.10-2.11} [Power Converters 3] (PowerConverters-1.7.10-2.11.jar) 
	UCHIJA	PracticalLogistics{0.2.4} [Practical Logistics] (Practical-Logistics-1.7.10-0.2.4.jar) 
	UCHIJA	ProjectBlue{1.1.6} [Project Blue] (ProjectBlue-1.1.6-mc1.7.10.jar) 
	UCHIJA	ProjRed|Transportation{4.7.0pre12.95} [ProjectRed Transportation] (ProjectRed-1.7.10-4.7.0pre12.95-Mechanical.jar) 
	UCHIJA	ProjRed|Compatibility{4.7.0pre12.95} [ProjectRed Compatibility] (ProjectRed-1.7.10-4.7.0pre12.95-Compat.jar) 
	UCHIJA	ProjRed|Integration{4.7.0pre12.95} [ProjectRed Integration] (ProjectRed-1.7.10-4.7.0pre12.95-Integration.jar) 
	UCHIJA	ProjRed|Fabrication{4.7.0pre12.95} [ProjectRed Fabrication] (ProjectRed-1.7.10-4.7.0pre12.95-Fabrication.jar) 
	UCHIJA	ProjRed|Illumination{4.7.0pre12.95} [ProjectRed Illumination] (ProjectRed-1.7.10-4.7.0pre12.95-Lighting.jar) 
	UCHIJA	ProjRed|Expansion{4.7.0pre12.95} [ProjectRed Expansion] (ProjectRed-1.7.10-4.7.0pre12.95-Mechanical.jar) 
	UCHIJA	quantumflux{1.7.10-1.3.4} [QuantumFlux] (QuantumFlux-1.7.10-1.3.4.jar) 
	UCHIJA	railcraft_cos{2.1.3} [Railcraft Cosmetic Additions] (Railcraft_Cosmetics-1.7.10-v2.1.3.jar) 
	UCHIJA	RandomThings{2.2.4} [Random Things] (RandomThings-2.2.4.jar) 
	UCHIJA	reborncore{1.1.0.15} [RebornCore] (RebornCore-1.1.0.15-universal.jar) 
	UCHIJA	reccomplex{0.9.7.1.1} [Recurrent Complex] (RecurrentComplex-0.9.7.1.1.jar) 
	UCHIJA	Redstonic{1.4.10} [Redstonic] (Redstonic-v1.4.11.jar) 
	UCHIJA	libsandstone{1.0.0} [libsandstone] (Reliquary-1.7.10-1.2.1.483.jar) 
	UCHIJA	xreliquary{1.2} [Reliquary] (Reliquary-1.7.10-1.2.1.483.jar) 
	UCHIJA	JAKJ_RedstoneInMotion{2.8.9} [Remain In Motion] (RemainInMotion-2.8.9.jar) 
	UCHIJA	RIO{2.4.0} [Remote IO] (RemoteIO-1.7.10-2.4.0-universal.jar) 
	UCHIJA	ResonantToolbox{1.0.9} [Resonant Toolbox] (ResonantToolbox-1.7.10-1.0.9.jar) 
	UCHIJA	simplyjetpacks{1.5.3} [Simply Jetpacks] (SimplyJetpacks-MC1.7.10-1.5.3.jar) 
	UCHIJA	rfdrills{1.7.3} [RFDrills] (RFDrills-1.7.10-1.7.3.jar) 
	UCHIJA	rftools{4.23} [RFTools] (rftools-4.23.jar) 
	UCHIJA	rfwindmill{0.7c} [RF Windmill] (rfwindmill-1.7.10-0.7c.jar) 
	UCHIJA	Roguelike{1.5.0} [Roguelike Dungeons] (roguelike-1.7.10-1.5.0b.jar) 
	UCHIJA	RouterReborn{1.2.0.43} [Router Reborn] (RouterReborn-1.7.10-1.2.0.43-universal.jar) 
	UCHIJA	runesofwizardry{1.7.10-0.3.1} [Runes of Wizardry] (Runes-of-Wizardry-1.7.10-0.3.1.jar) 
	UCHIJA	runicdungeons{1.1.7b} [Runic Dungeons] (RunicDungeons-1.1.7b.jar) 
	UCHIJA	cientificalchemy{1.0} [cientificalchemy] (ScientificAlchemy-1.7.10-1.3.jar) 
	UCHIJA	SGCraft{1.13.3} [Greg's SG Craft] (SGCraft-1.13.3-mc1.7.10.jar) 
	UCHIJA	SilentGems{1.3.14} [Silent's Gems] (SilentGems-1.7.10-1.3.14-172.jar) 
	UCHIJA	SilentPets{0.2.02} [Silent's Pets] (SilentPets-1.7.10-0.2.02-20.jar) 
	UCHIJA	flammpfeil.slashblade{mc1.7.10-r88} [SlashBlade] (SlashBlade-mc1.7.10-r88.jar) 
	UCHIJA	snad{1.7.10-1.6.01.31a} [Snad] (Snad-1.7.10-1.6.01.31a.jar) 
	UCHIJA	sodacantorches{01.07.01} [Sodacan Utilities] (sodacanutilities-01.07.01.jar) 
	UCHIJA	sodiumcraft{1.2} [SodiumCraft] (sodiumcraft-1.2.jar) 
	UCHIJA	SolarExpansion{1.6a} [Solar Expansion] (SolarExpansion-Basic-1.6a.jar) 
	UCHIJA	SolarFlux{1.7.10-0.8b} [Solar Flux] (SolarFlux-1.7.10-0.8b.jar) 
	UCHIJA	SSTOW{1.7.10-0.1-RC9-7} [Soul Shards: The Old Ways] (SoulShards-TOW-1.7.10-0.1-RC9-7.jar) 
	UCHIJA	SparksHammers{1.7.10-1.6} [Spark's Hammers] (SparksHammers-1.7.10-1.6.1.jar) 
	UCHIJA	SpecialAI{1.1.2} [Special AI] (SpecialAI-1.7.10-1.1.2.jar) 
	UCHIJA	squidless{0.6.1} [Squidless] (squidless-1.7.10-0.6.1.jar) 
	UCHIJA	bq_standard{2.0.130} [Standard Expansion] (StandardExpansion-2.0.130.jar) 
	UCHIJA	StevesFactoryManager{A93} [Steve's Factory Manager] (StevesFactoryManagerA93.jar) 
	UCHIJA	StevesAddons{0.10.16} [Steve's Addons] (StevesAddons-1.7.10-0.10.16.jar) 
	UCHIJA	StevesCarts{2.0.0.b18} [Steve's Carts 2] (StevesCarts2.0.0.b18.jar) 
	UCHIJA	StorageDrawers{1.7.10-1.10.9} [Storage Drawers] (StorageDrawers-1.7.10-1.10.9.jar) 
	UCHIJA	StorageDrawersForestry{1.7.10-1.1.2} [Storage Drawers: Forestry Pack] (StorageDrawers-Forestry-1.7.10-1.1.2.jar) 
	UCHIJA	StorageDrawersMisc{1.7.10-1.1.2} [Storage Drawers: Misc Pack] (StorageDrawers-Misc-1.7.10-1.1.2.jar) 
	UCHIJA	SuperMultiDrills{1.2.1b} [Super Multi-Drills] (SuperMultiDrills-1.7.10-1.2.1b.jar) 
	UCHIJA	TaintedMagic{r7.82} [Tainted Magic] (Tainted-Magic-r7.82.jar) 
	UCHIJA	TardisMod{0.994} [Tardis Mod] (tardismod-1.7.10-0.994-124-DS.jar) 
	UCHIJA	tcinventoryscan{1.0.11} [TC Inventory Scanning] (tcinventoryscan-mc1.7.10-1.0.11.jar) 
	UCHIJA	tcnodetracker{1.1.2} [TC Node Tracker] (tcnodetracker-1.7.10-1.1.2.jar) 
	UCHIJA	Techguns{0.1.2_alphatest4.1} [Techguns] (Techguns.beta.1.2_alphatest4.1.jar) 
	UCHIJA	techreborn{0.7.21.1131} [TechReborn] (TechReborn-1.7.10-0.7.21.1131-universal.jar) 
	UCHIJA	thaumcraftgates{1.4.2} [Thaumcraft Gates] (ThaumcraftGates-1.4.2.jar) 
	UCHIJA	ThaumcraftMobAspects{1.7.2-2A} [Thaumcraft Mob Aspects] (ThaumcraftMobAspects-1.7.2-2A.jar) 
	UCHIJA	thaumcraftneiplugin{@VERSION@} [Thaumcraft NEI Plugin] (thaumcraftneiplugin-1.7.10-1.7a.jar) 
	UCHIJA	thaumicbases{1.3.1710.2} [Thaumic Bases] (ThaumicBases-1.3.1710.4.jar) 
	UCHIJA	thaumicenergistics{1.1.3.0} [Thaumic Energistics] (thaumicenergistics-1.1.3.0.jar) 
	UCHIJA	ThaumicEquivalence{1.7.10-1.0.4} [Thaumic Equivalence] (ThaumicEquivalence-1.7.10-1.0.4.jar) 
	UCHIJA	thaumicexpansion{4.1.3} [Thaumic Expansion] (ThaumicExpansion-1.7.10-4.1.3.jar) 
	UCHIJA	thaumicinfusion{4.32} [Thaumic Infusion] (ThaumicInfusion-4.32.jar) 
	UCHIJA	thebetweenlands{1.0.6-alpha} [The Betweenlands] (TheBetweenlands-1.0.6-alpha-universal.jar) 
	UCHIJA	erebus{0.4.7} [Erebus] (TheErebus-0.4.7.jar) 
	UCHIJA	ThermalDynamics{1.7.10R1.2.1} [Thermal Dynamics] (ThermalDynamics-[1.7.10]1.2.1-172.jar) 
	UCHIJA	ThermalSmeltery{v1.1} [Thermal Smeltery] (ThermalSmeltery-Redux-v1.1.jar) 
	UCHIJA	TiCTooltips{1.2.5} [TiC Tooltips] (TiCTooltips-mc1.7.10-1.2.5.jar) 
	UCHIJA	tinker_io{release 1.5.0} [Tinker I/O] (tinker_io-1.7.10-release 1.5.0.jar) 
	UCHIJA	tis3d{1.4.0.78} [TIS-3D] (TIS-3D-MC1.7.10-1.4.0.78.jar) 
	UCHIJA	TMechworks{0.2.15.106} [Tinkers' Mechworks] (TMechworks-1.7.10-0.2.15.106.jar) 
	UCHIJA	Torcherino{2.2s} [Torcherino] (Torcherino-1.7.10-2.2s.jar) 
	UCHIJA	Translocator{1.1.2.16} [Translocator] (Translocator-1.7.10-1.1.2.16-universal.jar) 
	UCHIJA	trashslot{1.0.31} [TrashSlot] (trashslot-mc1.7.10-1.0.31.jar) 
	UCHIJA	TravellersGear{1.16.6} [Traveller's Gear] (TravellersGear-1.7.10-1.16.6.jar) 
	UCHIJA	bspkrsCore{6.16} [bspkrsCore] ([1.7.10]bspkrsCore-universal-6.16.jar) 
	UCHIJA	Treecapitator{1.7.10} [Treecapitator] (Treecapitator-universal-2.0.4.jar) 
	UCHIJA	uncrafted{2.2.0} [Uncrafted Mod] (Uncrafted 1.7.10 (v.2.2.0).jar) 
	UCHIJA	vending{1.2.3} [vending] (vending-v1.2.3.jar) 
	UCHIJA	voltzenginemodcompat{1.11.0.491} [Voltz Engine Mod Compatibility Loader] (VoltzEngine-1.7.10-1.11.0b491.jar) 
	UCHIJA	voltzenginemodflag{1.11.0.491} [VoltzEngine mod protection, flag, and region system] (VoltzEngine-1.7.10-1.11.0b491.jar) 
	UCHIJA	wailaplugins{MC1.7.10-0.2.0-25} [WAILA Plugins] (WAILAPlugins-MC1.7.10-0.2.0-25.jar) 
	UCHIJA	warpbook{2.0.null} [Warp Book] (warpbook-1.7.10_2.0.37.jar) 
	UCHIJA	witchery{0.24.1} [Witchery] (witchery-1.7.10-0.24.1.jar) 
	UCHIJA	witcherypatch{1.0.0} [WitcheryPatch] (WitcheryPatch-1.7.10-1.0.0.jar) 
	UCHIJA	WitchingGadgets{1.1.10} [Witching Gadgets] (WitchingGadgets-1.7.10-1.1.10.jar) 
	UCHIJA	worldedit{6.1.1} [WorldEdit] (worldedit-forge-mc1.7.10-6.1.1-dist.jar) 
	UCHIJA	xact{0.5.6} [XACT] (XACT-1.7.10-0.5.6.jar) 
	UCHIJA	XtraRecipes{3.0} [XtraRecipes] (XtraRecipes-3.0_1.7.10.jar) 
	UCHIJA	yegamolchattels{1.1.2} [Ye Gamol Chattels] (YeGamolChattels-1.1.2.jar) 
	UCHIJA	zettaindustries{1.1} [Zetta Industries] (zettaindustries-1.1-120.jar) 
	UCHIJA	ForgeMicroblock{1.2.0.347} [Forge Microblocks] (ForgeMultipart-1.7.10-1.2.0.347-universal.jar) 
	UCHIJA	McMultipart{1.2.0.347} [Minecraft Multipart Plugin] (ForgeMultipart-1.7.10-1.2.0.347-universal.jar) 
	UCHIJA	ForgeRelocation{0.0.1.4} [ForgeRelocation] (ForgeRelocation-1.7.10-0.0.1.4-universal.jar) 
	UCHIJA	MCFrames{1.0} [MCFrames] (ForgeRelocation-1.7.10-0.0.1.4-universal.jar) 
	UCHIJA	RelocationFMP{0.0.1.2} [RelocationFMP] (ForgeRelocationFMP-1.7.10-0.0.1.2-universal.jar) 
	UCHIJA	aobd{2.9.2} [Another One Bites The Dust] (AOBD-2.9.2.jar) 
	UCHIJA	denseores{1.0} [Dense Ores] (denseores-1.6.2.jar) 
	UCHIJA	technom{0.12.5} [Technomancy] (Technomancy+-+0.12.5+-+1.7.10.jar) 
	UD	equivalentenergisticsCore{0.8.3} [Equivalent Energistics Core] (minecraft.jar) 
	UD	MineFactoryReloaded|CompatAtum{1.7.10R2.8.1} [MFR Compat: Atum] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UD	MineFactoryReloaded|CompatBackTools{1.7.10R2.8.1} [MFR Compat: BackTools] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UD	MineFactoryReloaded|CompatChococraft{1.7.10R2.8.1} [MFR Compat: Chococraft] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UD	MineFactoryReloaded|CompatExtraBiomes{1.7.10R2.8.1} [MFR Compat: ExtraBiomes] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	UD	MineFactoryReloaded|CompatSufficientBiomes{1.7.10R2.8.1} [MFR Compat: Sufficient Biomes] (MineFactoryReloaded-[1.7.10]2.8.1-174.jar) 
	GL info: ' Vendor: 'Intel' Version: '4.0.0 - Build 10.18.10.4358' Renderer: 'Intel(R) HD Graphics 4000'
	OpenModsLib class transformers: [stencil_patches:FINISHED],[movement_callback:FINISHED],[player_damage_hook:FINISHED],[map_gen_fix:FINISHED],[gl_capabilities_hook:FINISHED],[player_render_hook:FINISHED]
	Class transformer null safety: found misbehaving transformers: me.guichaguri.betterfps.transformers.MathTransformer(me.guichaguri.betterfps.transformers.MathTransformer@374dc19) returned non-null result: 0,me.guichaguri.betterfps.transformers.EventTransformer(me.guichaguri.betterfps.transformers.EventTransformer@35d6a203) returned non-null result: 0
	AE2 Version: beta rv3-beta-6 for Forge 10.13.4.1448
	CoFHCore: -[1.7.10]3.1.4-329
	ThermalFoundation: -[1.7.10]1.2.6-118
	Mantle Environment: Environment healthy.
	ThermalExpansion: -[1.7.10]4.1.5-248
	MineFactoryReloaded: -[1.7.10]2.8.1-174
	TConstruct Environment: Environment healthy.
	RedstoneArsenal: -[1.7.10]1.1.2-92
	NetherOres: -[1.7.10]2.3.1-22
	ThermalDynamics: -[1.7.10]1.2.1-172
	List of loaded APIs: 
		* AbyssalCraftAPI (1.7) from AbyssalCraft-1.7.10-1.9.1.3-FINAL.jar
		* ActuallyAdditionsAPI (3) from ActuallyAdditions-1.7.10-r21.jar
		* ae2wct|API (1.7.10-rv3-1.8.6b) from WirelessCraftingTerminal-1.7.10-rv3-1.8.7.9b.jar
		* AgriCraftAPI (1.0) from AgriCraft-1.7.10-1.5.0.jar
		* AncientWarfareAPI (1.0) from ancientwarfare-2.4.115-beta-MC1.7.10-FULL.jar
		* API_NEK (1.2.0) from (client)NotEnoughKeys-1.7.10-3.0.0b45-dev-universal.jar
		* AppleCoreAPI (3.1.0) from AppleCore-mc1.7.10-3.1.1.jar
		* appliedenergistics2|API (rv2) from ThaumicTinkerer-2.5-1.7.10-164.jar
		* AromaBackupAPI (1.0) from AromaBackup-1.7.10-0.1.0.0.jar
		* AuraEnergyAPI (1.0.6) from DimensionalCore-1.7.10-1.0.7.jar
		* Baubles|API (1.0.1.10) from ThermalFoundation-[1.7.10]1.2.6-118.jar
		* bcadditionsAPI (2.1.1) from BuildcraftAdditions-1.7.10-2.2.5.jar
		* BetterAchievements|API (0.1.0) from BetterAchievements-1.7.10-0.1.0.jar
		* BetterQuesting|API (2.6) from BetterQuesting-2.0.233.jar
		* BloodMagicAPI (1.3.3-13) from BloodMagic-1.7.10-1.3.3-17.jar
		* Boilerplate|API (1) from boilerplate-1.7.10-6.3.0.81-universal.jar
		* BotaniaAPI (76) from Botania r1.8-249.jar
		* BuildCraftAPI|blocks (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|blueprints (1.5) from buildcraft-7.1.23.jar
		* BuildCraftAPI|boards (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|core (1.0) from extrautilities-1.2.12.jar
		* BuildCraftAPI|crops (1.1) from Railcraft_1.7.10-9.12.2.0.jar
		* BuildCraftAPI|events (2.0) from buildcraft-7.1.23.jar
		* BuildCraftAPI|facades (1.1) from buildcraft-7.1.23.jar
		* BuildCraftAPI|filler (4.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|fuels (2.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|gates (4.1) from buildcraft-7.1.23.jar
		* BuildCraftAPI|items (1.1) from Railcraft_1.7.10-9.12.2.0.jar
		* BuildCraftAPI|library (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|lists (1.0) from buildcraft-7.1.23.jar
		* BuildCraftAPI|power (1.3) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|recipes (2.1) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|robotics (3.0) from buildcraft-7.1.23.jar
		* BuildCraftAPI|statements (1.1) from Railcraft_1.7.10-9.12.2.0.jar
		* BuildCraftAPI|tablet (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|tiles (1.2) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|tools (1.0) from SolarExpansion-Basic-1.6a.jar
		* BuildCraftAPI|transport (4.1) from Railcraft_1.7.10-9.12.2.0.jar
		* CalculatorAPI (1.7.10 - 1.1) from Calculator-1.7.10-1.9.11.jar
		* CalendarAPI|API (1.2) from Calendar-1.7.10-1.0-4.jar
		* CarpentersBlocks|API (3.3.7) from Carpenter_s Blocks v3.3.8.1 - MC 1.7.10.jar
		* ChiselAPI (0.1.1) from Chisel-2.9.5.11.jar
		* ChiselAPI|Carving (0.1.1) from Chisel-2.9.5.11.jar
		* ChiselAPI|Rendering (0.1.1) from Chisel-2.9.5.11.jar
		* CoFHAPI (1.7.10R1.1.0) from SonarCore-1.7.10-1.1.3.jar
		* CoFHAPI|block (1.7.10R1.1.0) from NuclearCraft-1.9g--1.7.10.jar
		* CoFHAPI|core (1.7.10R1.1.0) from NuclearCraft-1.9g--1.7.10.jar
		* CoFHAPI|energy (1.7.10R1.1.0) from NuclearCraft-1.9g--1.7.10.jar
		* CoFHAPI|fluid (1.7.10R1.1.0) from SonarCore-1.7.10-1.1.3.jar
		* CoFHAPI|inventory (1.7.10R1.0.12) from EngineersToolbox-1.2.3.0-BETA.jar
		* CoFHAPI|item (1.7.10R1.0.2) from boilerplate-1.7.10-6.3.0.81-universal.jar
		* CoFHAPI|items (1.7.10R1.0.3) from SolarExpansion-Basic-1.6a.jar
		* CoFHAPI|modhelpers (1.7.10R1.0.1) from SilentGems-1.7.10-1.3.14-172.jar
		* CoFHAPI|tileentity (1.7.10R1.1.0) from SonarCore-1.7.10-1.1.3.jar
		* CoFHAPI|transport (1.7.10R1.0.13) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* CoFHAPI|world (1.7.10R1.1.0) from NuclearCraft-1.9g--1.7.10.jar
		* CoFHLib (1.7.10R1.2.1) from CoFHCore-[1.7.10]3.1.4-329.jar
		* CoFHLib|audio (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* CoFHLib|gui (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* CoFHLib|gui|container (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* CoFHLib|gui|element (1.7.10R1.2.1) from CoFHCore-[1.7.10]3.1.4-329.jar
		* CoFHLib|gui|element|listbox (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* CoFHLib|gui|slot (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* CoFHLib|inventory (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* CoFHLib|render (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* CoFHLib|render|particle (1.7.10R1.2.1) from CoFHCore-[1.7.10]3.1.4-329.jar
		* CoFHLib|util (1.7.10R1.2.1) from CoFHCore-[1.7.10]3.1.4-329.jar
		* CoFHLib|util|helpers (1.7.10R1.2.1) from CoFHCore-[1.7.10]3.1.4-329.jar
		* CoFHLib|util|position (1.7.10R1.2.1) from CoFHCore-[1.7.10]3.1.4-329.jar
		* CoFHLib|world (1.7.10R1.2.1) from CoFHCore-[1.7.10]3.1.4-329.jar
		* CoFHLib|world|feature (1.7.10R1.0.4B1) from EnderTech-1.7.10-0.3.2.405.jar
		* compactstorage (v2.0.0a) from compactstorage-1.7.10-release-2.1.0-lts.21-universal.jar
		* ComputerCraft|API (1.75) from ComputerCraft1.75.jar
		* ComputerCraft|API|FileSystem (1.75) from Traincraft-4.4.1_020.jar
		* ComputerCraft|API|Lua (1.75) from ComputerCraft1.75.jar
		* ComputerCraft|API|Media (1.74) from EngineersToolbox-1.2.3.0-BETA.jar
		* ComputerCraft|API|Peripheral (1.75) from Traincraft-4.4.1_020.jar
		* ComputerCraft|API|Permissions (1.75) from ComputerCraft1.75.jar
		* ComputerCraft|API|Redstone (1.75) from Traincraft-4.4.1_020.jar
		* ComputerCraft|API|Turtle (1.74) from EngineersToolbox-1.2.3.0-BETA.jar
		* CoroAI|dynamicdifficulty (1.0) from coroutil-1.7.10-1.1.6.jar
		* CraftingTweaks|API (4.1) from craftingtweaks-mc1.7.10-1.0.88.jar
		* CSLib|API (0.3.0) from Decocraft-2.4.2_1.7.10.jar
		* DLDungeonsAPI (1.4) from DoomlikeDungeons-1.11.0.1-MC1.7.10.jar
		* DraconicEvolution|API (1.2) from Draconic-Evolution-1.7.10-1.0.2h.jar
		* EnderIOAPI (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* EnderIOAPI|Redstone (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* EnderIOAPI|Teleport (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* EnderIOAPI|Tools (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* fluxedtrinketsAPI (0.53) from Fluxed Trinkets-1.7.10-1.0.54.jar
		* ForestryAPI|apiculture (4.8.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|arboriculture (4.2.1) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|circuits (3.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|core (5.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|farming (2.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|food (1.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|fuels (2.0.1) from TechReborn-1.7.10-0.7.21.1131-universal.jar
		* ForestryAPI|genetics (4.7.1) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|hives (4.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|lepidopterology (1.3.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|mail (3.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|multiblock (3.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|recipes (5.4.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|storage (3.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|world (2.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForgeRelocation|API (0.0.1.4) from ForgeRelocation-1.7.10-0.0.1.4-universal.jar
		* Fossils and Archeology Revival API (7.3.1) from fossilsarcheology-7.3.2.jar
		* Galacticraft API (1.1) from GalacticraftCore-1.7-3.0.12.504.jar
		* GameAnalyticsAPI (1.1) from AuraCascade-557.jar
		* gendustryAPI (2.3.0) from gendustry-1.6.3.132-mc1.7.10.jar
		* Guide-API|API (1.7.10-1.0.1-29) from Guide-API-1.7.10-1.0.1-29.jar
		* IC2API (1.0) from SonarCore-1.7.10-1.1.3.jar
		* ImmersiveEngineering|API (1.0) from ImmersiveEngineering-0.7.7.jar
		* inpure|api (1.7) from INpureCore-[1.7.10]1.0.0B9-62.jar
		* MagneticraftAPI (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Computer (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Computer|PreFab (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|ConveyorBelt (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|ConveyorBelt|PreFab (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Electricity (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Electricity|PreFab (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Heat (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Heat|PreFab (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Kinetic (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Pressure (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Pressure|PreFab (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Radiation (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Recipes (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Steel (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Tools (2.0.3) from magneticraft-0.6.1-final.jar
		* MagneticraftAPI|Util (2.0.3) from magneticraft-0.6.1-final.jar
		* MatterOverdrive|API (0.4.1) from MatterOverdrive-1.7.10-0.4.2.jar
		* McJtyLib (1.8.1) from mcjtylib-1.8.1.jar
		* MekanismAPI|core (9.0.0) from Mekanism-1.7.10-9.1.1.1031.jar
		* MekanismAPI|energy (9.0.0) from NuclearCraft-1.9g--1.7.10.jar
		* MekanismAPI|gas (9.0.0) from NuclearCraft-1.9g--1.7.10.jar
		* MekanismAPI|infuse (9.0.0) from NuclearCraft-1.9g--1.7.10.jar
		* MekanismAPI|laser (9.0.0) from Mekanism-1.7.10-9.1.1.1031.jar
		* MekanismAPI|reactor (9.0.0) from Mekanism-1.7.10-9.1.1.1031.jar
		* MekanismAPI|recipe (9.0.0) from Mekanism-1.7.10-9.1.1.1031.jar
		* MekanismAPI|transmitter (9.0.0) from NuclearCraft-1.9g--1.7.10.jar
		* MekanismAPI|util (9.0.0) from NuclearCraft-1.9g--1.7.10.jar
		* MetallurgyAPI (2.0.0) from Metallurgy-1.7.10-4.0.6.80.jar
		* moarcarts|API (1.0) from moarcarts-1.7.10-1.2.4-11.jar
		* neresources|API (1.0) from NotEnoughResources-1.7.10-0.1.0-128.jar
		* NHWrenchAPI (1.7.10V1.0.0) from nhwrench-1.7.10-3.1.6.jar
		* NuclearControlAPI (v1.0.5) from IC2NuclearControl-2.4.3a.jar
		* OpenBlocks|API (1.1) from OpenBlocks-1.7.10-1.6.jar
		* OpenComputersAPI|Component (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|Core (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|Driver (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|Driver|Item (6.0.0-alpha) from OpenComputers-MC1.7.10-1.7.4.1265-universal.jar
		* OpenComputersAPI|Event (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|FileSystem (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|Internal (6.0.0-alpha) from OpenComputers-MC1.7.10-1.7.4.1265-universal.jar
		* OpenComputersAPI|Machine (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|Manual (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|Network (5.6.4) from CD4017BE_lib-1.7.10-2.7.4b.jar
		* OpenComputersAPI|Prefab (6.0.0-alpha) from OpenComputers-MC1.7.10-1.7.4.1265-universal.jar
		* OpenPeripheralAddonsApi (1.0) from OpenPeripheralAddons-1.7.10-0.6.jar
		* OpenPeripheralApi (3.4.2) from OpenPeripheralCore-1.7.10-1.4.jar
		* OriginScrewdriverApi (1.0.0) from Origin-1.7.10-8.0.3.jar
		* PneumaticCraftApi (1.0) from PneumaticCraft-1.7.10-1.12.7-152-universal.jar
		* PracticalLogisticsAPI (1.4) from Practical-Logistics-1.7.10-0.2.4.jar
		* pressureAPI (1.3.0.fix1) from pressure-1.3.0.fix1-mc1.7.10.jar
		* ProjectEAPI (7) from ProjectE-1.7.10-PE1.10.1.jar
		* RailcraftAPI|bore (1.0.0) from Traincraft-4.4.1_020.jar
		* RailcraftAPI|carts (1.6.0) from Traincraft-4.4.1_020.jar
		* RailcraftAPI|core (1.3.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|crafting (1.0.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|electricity (1.6.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|events (1.0.0) from Railcraft_1.7.10-9.12.2.0.jar
		* RailcraftAPI|fuel (1.0.0) from Railcraft_1.7.10-9.12.2.0.jar
		* RailcraftAPI|helpers (1.1.0) from Railcraft_1.7.10-9.12.2.0.jar
		* RailcraftAPI|items (1.0.0) from Railcraft_1.7.10-9.12.2.0.jar
		* RailcraftAPI|locomotive (1.0.1) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|signals (2.3.0) from Traincraft-4.4.1_020.jar
		* RailcraftAPI|tracks (2.0.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* reborncoreAPI (1.1.0.15) from RebornCore-1.1.0.15-universal.jar
		* runesofwizardry|API (@MOD_VERSION@) from Runes-of-Wizardry-1.7.10-0.3.1.jar
		* SecurityCraftAPI (1.2.2) from [1.7.10] SecurityCraft v1.8.12.jar
		* StorageDrawersAPI (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|config (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|event (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|inventory (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|pack (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|registry (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|render (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|storage (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* StorageDrawersAPI|storage-attribute (1.7.10-1.2.0) from StorageDrawers-1.7.10-1.10.9.jar
		* techrebornAPI (0.7.21.1131) from TechReborn-1.7.10-0.7.21.1131-universal.jar
		* Thaumcraft|API (4.2.2.0) from tardismod-1.7.10-0.994-124-DS.jar
		* thaumicenergistics|API (1.1) from thaumicenergistics-1.1.3.0.jar
		* tis3dAPI (1.4.0.78) from TIS-3D-MC1.7.10-1.4.0.78.jar
		* TravellersGear|API (1.0) from TravellersGear-1.7.10-1.16.6.jar
		* TSteelworksAPI (1.2) from TSteelworks-1.7.10-1.1.2-20.jar
		* VoltzEngineAPI (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|crafting-items (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|data (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|energy (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|energy-items (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|event (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|explosive-items (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|explosives (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|items (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|recipe (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|tile (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|tools (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* VoltzEngineAPI|weapons (0.11.0) from VoltzEngine-1.7.10-1.11.0b491.jar
		* WailaAPI (1.2) from DimensionalCore-1.7.10-1.0.7.jar
		* waterhooks|API (1.0) from waterhooks-1.2.1.jar
		* XACT-API (1) from XACT-1.7.10-0.5.6.jar
	Chisel: Errors like "[FML]: Unable to lookup ..." are NOT the cause of this crash. You can safely ignore these errors. And update forge while you're at it.
	EnderIO: Found the following problem(s) with your installation:
                  * The RF API that is being used (1.7.10R1.0.2 from <unknown>) differes from that that is reported as being loaded (1.7.10R1.1.0 from NuclearCraft-1.9g--1.7.10.jar).
                    It is a supported version, but that difference may lead to problems.
                 This may have caused the error. Try reproducing the crash WITHOUT this/these mod(s) before reporting it.
	Stencil buffer state: Function set: GL30, pool: forge, bits: 8
	AE2 Integration: IC2:ON, RotaryCraft:OFF, RC:ON, BuildCraftCore:ON, BuildCraftTransport:ON, BuildCraftBuilder:ON, RF:ON, RFItem:ON, MFR:ON, DSU:ON, FZ:OFF, FMP:ON, RB:OFF, CLApi:OFF, Waila:ON, InvTweaks:ON, NEI:ON, CraftGuide:OFF, Mekanism:ON, ImmibisMicroblocks:OFF, BetterStorage:OFF, OpenComputers:ON, PneumaticCraft:ON
	Launched Version: forge-10.13.4.1614
	LWJGL: 2.9.1
	OpenGL: Intel(R) HD Graphics 4000 GL version 4.0.0 - Build 10.18.10.4358, Intel
	GL Caps: Using GL 1.3 multitexturing.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Anisotropic filtering is supported and maximum anisotropy is 16.
Shaders are available because OpenGL 2.1 is supported.

	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: []
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Anisotropic Filtering: Off (1)
