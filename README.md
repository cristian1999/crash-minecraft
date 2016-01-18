# crash-minecraft

Description: Unexpected error

java.lang.RuntimeException: Cannot Hotload Dim: Overworld is not Loaded!
	at net.minecraftforge.common.DimensionManager.initDimension(DimensionManager.java:239)
	at net.minecraft.server.MinecraftServer.func_71218_a(MinecraftServer.java:746)
	at Config.getWorldServer(Config.java:1806)
	at RandomMobs.entityLoaded(RandomMobs.java:42)
	at net.minecraft.client.renderer.RenderGlobal.func_72703_a(RenderGlobal.java:2355)
	at net.minecraft.world.World.func_72923_a(World.java:1589)
	at net.minecraft.client.multiplayer.WorldClient.func_72923_a(WorldClient.java:206)
	at net.minecraft.world.World.func_72838_d(World.java:1580)
	at net.minecraft.client.multiplayer.WorldClient.func_72838_d(WorldClient.java:184)
	at net.minecraft.client.multiplayer.WorldClient.func_73027_a(WorldClient.java:246)
	at cpw.mods.fml.client.FMLClientHandler.spawnEntityIntoClientWorld(FMLClientHandler.java:461)
	at cpw.mods.fml.common.FMLCommonHandler.spawnEntityIntoClientWorld(FMLCommonHandler.java:339)
	at cpw.mods.fml.common.network.EntitySpawnPacket.execute(EntitySpawnPacket.java:194)
	at cpw.mods.fml.common.network.FMLNetworkHandler.handleFMLPacket(FMLNetworkHandler.java:116)
	at cpw.mods.fml.common.network.FMLNetworkHandler.handlePacket250Packet(FMLNetworkHandler.java:81)
	at net.minecraft.client.multiplayer.NetClientHandler.func_72501_a(NetClientHandler.java:1651)
	at net.minecraft.network.packet.Packet250CustomPayload.func_73279_a(SourceFile:61)
	at net.minecraft.network.MemoryConnection.func_74428_b(MemoryConnection.java:89)
	at net.minecraft.client.Minecraft.func_71407_l(Minecraft.java:1967)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:910)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:838)
	at net.minecraft.client.main.Main.main(SourceFile:101)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:131)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:27)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at net.minecraftforge.common.DimensionManager.initDimension(DimensionManager.java:239)
	at net.minecraft.server.MinecraftServer.func_71218_a(MinecraftServer.java:746)
	at Config.getWorldServer(Config.java:1806)
	at RandomMobs.entityLoaded(RandomMobs.java:42)
	at net.minecraft.client.renderer.RenderGlobal.func_72703_a(RenderGlobal.java:2355)
	at net.minecraft.world.World.func_72923_a(World.java:1589)
	at net.minecraft.client.multiplayer.WorldClient.func_72923_a(WorldClient.java:206)
	at net.minecraft.world.World.func_72838_d(World.java:1580)
	at net.minecraft.client.multiplayer.WorldClient.func_72838_d(WorldClient.java:184)
	at net.minecraft.client.multiplayer.WorldClient.func_73027_a(WorldClient.java:246)
	at cpw.mods.fml.client.FMLClientHandler.spawnEntityIntoClientWorld(FMLClientHandler.java:461)
	at cpw.mods.fml.common.FMLCommonHandler.spawnEntityIntoClientWorld(FMLCommonHandler.java:339)
	at cpw.mods.fml.common.network.EntitySpawnPacket.execute(EntitySpawnPacket.java:194)
	at cpw.mods.fml.common.network.FMLNetworkHandler.handleFMLPacket(FMLNetworkHandler.java:116)
	at cpw.mods.fml.common.network.FMLNetworkHandler.handlePacket250Packet(FMLNetworkHandler.java:81)
	at net.minecraft.client.multiplayer.NetClientHandler.func_72501_a(NetClientHandler.java:1651)
	at net.minecraft.network.packet.Packet250CustomPayload.func_73279_a(SourceFile:61)
	at net.minecraft.network.MemoryConnection.func_74428_b(MemoryConnection.java:89)

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [GCCorePlayerSP['crischulo84'/393, l='MpServer', x=-116,42, y=101,20, z=-70,13]]
	Chunk stats: MultiplayerChunkCache: 9
	Level seed: 0
	Level generator: ID 00 - default, ver 1. Features enabled: false
	Level generator options: 
	Level spawn location: World: (-96,64,248), Chunk: (at 0,4,8 in -6,15; contains blocks -96,0,240 to -81,255,255), Region: (-1,0; contains chunks -32,0 to -1,31, blocks -512,0,0 to -1,255,511)
	Level time: 474986 game time, 625123 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
	Forced entities: 2 total; [GCCorePlayerSP['crischulo84'/393, l='MpServer', x=-116,42, y=101,20, z=-70,13], EntityRustMonster['Rust Monster'/394, l='MpServer', x=-115,53, y=17,00, z=-79,00]]
	Retry entities: 0 total; []
	Server brand: fml,forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:440)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2312)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:863)
	at net.minecraft.client.main.Main.main(SourceFile:101)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:131)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:27)

-- System Details --
Details:
	Minecraft Version: 1.6.4
	Operating System: Windows 8.1 (amd64) version 6.3
	Java Version: 1.7.0_80, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 246889592 bytes (235 MB) / 748683264 bytes (714 MB) up to 954728448 bytes (910 MB)
	Mod Pack: Unknown / None
	LiteLoader Mods: 3 loaded mod(s)
          - VoxelPacket version 2.0.4
          - VoxelMenu version 3.0.7
          - VoxelLib version 2.1.0
	JVM Flags: 2 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx1G
	AABB Pool Size: 1 (56 bytes; 0 MB) allocated, 1 (56 bytes; 0 MB) used
	Suspicious classes: FML and Forge are installed
	IntCache: cache: 0, tcache: 0, allocated: 1, tallocated: 63
	FML: 
	mcp{8.09} [Minecraft Coder Pack] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	FML{6.4.49.965} [Forge Mod Loader] (minecraftforge-9.11.1.965.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	Forge{9.11.1.965} [Minecraft Forge] (minecraftforge-9.11.1.965.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	CodeChickenCore{0.9.0.9} [CodeChicken Core] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	Micdoodlecore{} [Micdoodle8 Core] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	NotEnoughItems{1.6.1.9} [Not Enough Items] (NotEnoughItems 1.6.1.9.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	PlayerAPI{1.1} [Player API] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	advancedgenetics{v1.4.3} [Advanced Genetics] (Advancedgenetics-1.4.3-1.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	Autoutils{1.0.1} [Autoutils] (Autoutils-1.6.4-1.0.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	Backpack{1.28.37} [Backpack] (Backpack-1.28.37-1.6.x.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	BetterDungeons{2.4} [Chocolate quest] (BetterDungeons2091.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	BiblioCraft{1.5.5} [BiblioCraft] (BiblioCraft[v1.5.5].zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	Botania{beta-16} [Botania] (Botania beta-16.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	ConfigMod{v1.0} [Extended Mod Config] (ConfigMod for MC v1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	CopiousDogs{alpha-1.1.2} [Copious Dogs] (Copious-dogs-alpha-1.1.2.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	CoroAI{v1.0} [CoroAI] (CoroUtil for MC v1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	creeperspecies{1.6.2} [Creeper Species] (Creeperspecies_1.6.2.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	wonderfulwands{1.1.0} [Cyano's Wonderful Wands] (CyanosWonderfulWands-1.1.0.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	DamageIndicatorsMod{2.9.2.4} [Damage Indicators] (DamageIndicatorsv2.9.2.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	props{1.9a} [DecoCraft] (DecoCraft1.6.4 V1.9b.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	deconstruction{2.0.1} [The Deconstruction Mod] (Deconstruction[v2.0.1].jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	digitalxp{0.1.2c} [DigitalXP] (Digitalxp-0.1.2c.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	dungeonmobs{3.0.5} [Dungeon Mobs] (Dungeon Mobs v3.0.5.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	TDS_EL{1.0.0} [Elementals] (Elementals 1.0.0 fixed.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	eplus{1.16.5b} [Enchanting Plus] (EnchantingPlus-1.16.5.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	eternalfrost{1.5b1} [Eternal Frost] (EternalFrost.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	evilcraft{0.4.1b} [EvilCraft] (EvilCraft-1.6.4-0.4.1b-51.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	ExtendedRenderer{v1.0} [Extended Renderer] (ExtendedRenderer for MC v1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	farlanders{1.1c} [The Farlanders] (Farlanders_v1.1c.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	LegendaryBeasts{a1.6.4.0} [Legendary Beasts] (Forge_LegendaryBeastsAlpha1.6.4.0.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	fossil{1.6.4 Build 6.4} [Fossils and Archeology Revival] (Fossils_Archeology_Revival-1.6.4_Build-6.4.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	UniversalElectricity{3.1.0} [Universal Electricity] (Universal-Electricity-3.1.0.115-core.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	ResonantEngine{@MAJOR@.@MINOR@.@REVIS@} [ResonantEngine] (Resonant-Engine-Development-1.2.0.266-universal.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	ICBM{1.4.2} [ICBM] (ICBM-1.4.2.386.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	ICBM|Sentry{1.4.2} [ICBM Sentry] (ICBM-1.4.2.386.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	ICBM|Explosion{1.4.2} [ICBM Explosion] (ICBM-1.4.2.386.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	GalacticraftCore{2.0.14} [Galacticraft Core] (Galacticraft-1.6.4-2.0.14.1084.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	GalacticraftMars{2.0.14} [Galacticraft Mars] (Galacticraft-Planets-1.6.4-2.0.14.1084.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	GraveStone{2.8.3} [GraveStone] (GraveStone_2.8.3.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	GrimoireGaia2{1.8.2} [§2Grimoire of Gaia 2] (GrimoireofGaia2(1.8.2c).zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	HostileWorlds{0.4.3} [Hostile Worlds] (Hostile Worlds v0.4.3 Alpha Mod for MC v1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	InfernalMobs{1.4.4} [Infernal Mobs] (InfernalMobs_1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	mca{3.6.1} [Minecraft Comes Alive] (MCA-3.6.1 MC-1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	meteors{2.11.2} [Falling Meteors] (Meteors_Mod_V2.11.2.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	BuildMod{v1.0} [Build Mod] (ModBuild for MC v1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	necromancy{1.5} [Necromancy] (Necromancy_1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	NEIPlugins{1.1.0.6} [NEI Plugins] (NEIPlugins-1.1.0.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	NetherX{1.2.2} [NetherX] (NetherX 1.3 for MC 1.6.4.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	ParticleMan{v1.0} [Particle Man] (Particle Man v1.4 Mod for MC v1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	PartyMod{Beta-V1.2} [Party Mod] (PartyMod-Beta-V1.2) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	mod_ReiMinimap{v3.4_01 [1.6.2]} [mod_ReiMinimap] (ReiMinimap_v3.4_01.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	AS_Ruins{11.0} [Ruins Spawning System] (Ruins_1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	awger_SmallBoat{0.10.6} [SmallBoat] (smallboats.0.10.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	awger_Punt{0.10.6} [Punt] (smallboats.0.10.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	awger_Whitehall{0.10.6} [Whitehall] (smallboats.0.10.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	awger_Hoy{0.10.6} [Hoy] (smallboats.0.10.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	mod_SmartMoving{14.6} [Smart Moving] (Smart Moving Universal for ModLoader or Minecraft Forge or MCPC+.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	mod_SmartRender{1.1} [Smart Render] (Smart Moving Universal for ModLoader or Minecraft Forge or MCPC+.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	Statues{2.1.1} [Statues] (statues-1.6.4-2.1.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	TF2Teleporter{1.6.4} [TF2 Teleporter] (TF2_Teleporter_1.6.4a.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	lionking{v1.13 for Minecraft 1.6.4} [The Lion King Mod] (The Lion King Mod v1.13.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	turtle{1.6.4} [Trotuman] (Trotuman_1.6.2-1.6.4.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	taverns{2.1.6-3} [Village Taverns] (VillageTaverns-2.1.6-3.15.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
	weaponmod{1.6.2 v1.13.6} [Balkon's WeaponMod] (WeaponMod.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available->Available
