### 彩虹引擎服务端架构图
---

WolServer（服务器端目录） 

├ DB

│└ GameLoad.DB (物品数据库) 

│　　├ Dragon （龙王属性数据库）

│　　├ Evil （心魔配置数据库）

│　　├ flyGoblin （妖士天人属性数据库） 

│　　├ flyTaos （道士天人属性数据库）

│　　├ flyWarr （战士天人属性数据库）

│　　├ flyWizard （法师天人属性数据库）

│　　├ pflyTaos （道士元神飞升属性数据库）

│　　├ pflyWarr （战士元神飞升属性数据库）

│　　├ pflyWizard （法师元神飞升属性数据库）

│　　├ Goblin （妖士属性数据库）

│　　├ Goblin_YaoDan （妖士妖丹属性数据库）

│　　├ Magic （技能数据库）

│　　├ Monster （怪物数据库）

│　　├ StdItems （物品数据库）

│　　├ TaoistPet （道士宝宝属性数据库）

│　　├ Taos （道士属性数据库-飞升前）

│　　├ Tiger （虎王属性数据库）

│　　├ Warr （战士属性数据库-飞升前）

│　　├ Wizard （法师属性数据库-飞升前）

│　　├ MentalWarr （天元心法-战士）

│　　├ MentalTaos （天元心法-道士）

│　　├ MentalWizard （天元心法-法师）

│　　└ Suite （套装属性数据库）

│
├ DBServer （数据库服务器目录）

│　├ Backup

│　├ ClearLog

│　├ Connection 

│　├ FDB

│　│　└ GameData.DB

│　│　　├ TBL_ACHIEVEMENT（成就数据表）

│　│　　├ TBL_BONUSABILITY（属性点、炼体属性表）

│　│　　├ TBL_CHARABILITY（人物扩展属性数据表）

│　│　　├ TBL_CHARACTER（人物基础属性数据表） 

│　│　　├ TBL_ITEM（人物装备和相关物品数据表）

│　│　　├ TBL_MAGIC（人物技能数据表）

│　│　　├ TBL_PETSELL（宠物摆摊数据表）

│　│　　├ TBL_QUEST（任务标记、人物扩展变量表） 

│　│　　├ TBL_SOCIALITY（人物社交信息表）

│　│　　├ TBL_TASK（任务数据表）

│　│　　├ TBL_CONSIGNBENEFITS（寄售收益数据表）

│　│　　└ TBL_CONSIGNITEMS（寄售物品数据表）

│　├ Log

│　├ !addrtable.txt

│　├ !serverinfo.txt

│　├ DBServer.exe（数据库服务器程序） 

│　├ dbsrc.ini

│　├ WhiteList.txt

│　└ CustomTableList（自定义数据表）

│
├ LoginSrv （帐号服务器目录）

│　├ ChrLog

│　├ CountLog 

│　├ !addrtable.txt （登录路由表）

│　├ !serveraddr.txt （允许连接IP列表）

│　├ LoginSrv.exe （登录服务器程序）

│　├ Logsrv.ini （登录服务器配置文件） 

│　├ IDDB

│　│　└ IDDB.DB（帐号数据库）

│　│　　└ TBL_ACCOUNT（玩家帐号信息表）

│　├ IdLog

│　├ !ResServerList.txt（客户端资源服务器IP列表）

│　└ !UserLimit.txt

│

├ LogServer （游戏日志服务器目录）

│ 　├ BaseDir （游戏日志保存目录）

│ 　├ LogData.ini （游戏日志服务器配置文件）

│　 └ LogDataServer.exe （游戏日志服务器程序）

│

├ Mir200 （游戏引擎程序目录）

│　 ├ Castle

│ 　│　 ├ List.txt （沙城目录文件,里面内容为数字0）

│ 　│　 └ 0（0的文件夹,保存沙城相关配置）

│ 　│　　 ├ SabukW.txt（沙城配置文件）

│ 　│　　 └ AttackSabukWall.txt（攻城记录） 

│ 　│ 

│ 　├ Config

│ 　│　 ├ achievement.xml（成就系统配置）

│　 │ 　├ BaoShi.xml（宝石属性配置）

│ 　│ 　├ Command.ini（游戏GM命令配置）

│　 │ 　├ Constellation.xml（星宿属性配置）

│　 │ 　├ ConstellationExps.ini（星宿等级配置） 

│　 │ 　├ GlobalVals.xml（G和A变量保存文件）

│　 │ 　├ GoblinPellet.xml（妖丹技能配置）

│ 　│　 ├ ItemCfg.ini（龙纹钢等级经验配置）

│ 　│ 　├ LianTiCfg.xml（炼体属性配置）

│ 　│ 　├ OfficerExps.ini（仙官等级经验配置）

│ 　│ 　├ PetExp.ini（宠物升级经验配置）

│ 　│ 　├ MagicSkill.xml（魔法技能配置，下载地址：Www.YyCh3.Com）

│ 　│　 ├ wenpeiconfig.xml（纹佩属性配置）

│　 │　 ├ Exps.ini（人物升级经验）

│　 │ 　├ String.ini（游戏内提示文字配置）

│　 │ 　├ leilian.xml（雷炼属性配置）

│　 │ 　├ MilitaryMedal.xml（铁血勋章属性配置）

│　 │ 　├ MilitaryRank.xml（军衔属性配置）

│　 │ 　├ PneumaTuPoCfg.Xml（元神突破属性配置）

│　 │ 　├ InsightPetCfg.json（灵兽顿悟属性配置）

│　 │ 　├ xuewei_daoshi.xml（道士修为属性配置）

│　 │ 　├ xuewei_fashi.xml（法师修为属性配置）

│　 │ 　├ xuewei_zhanshi.xml（战士修为属性配置）

│　 │ 　├ xuewei_yaoshi.xml（妖士修为属性配置）

│　 │ 　├ xuewei_lingqiang.xml (灵枪区境界系统)

│　 │ 　├ FengMotuSuit.xml（封魔图属性配置）

│　 │ 　├ Enchantitems.xml（符文技能配置）

│　 │ 　├ RepressDemon.xml（镇魔珠属性配置）

│　 │ 　├ RepressDemonEquips.xml（镇魔装备系统属性配置）

│　 │ 　├ RepressDemonwings.xml（镇魔羽翼属性配置）

│　 │ 　├ Fabao.xml（法宝属性参数控制、法宝升级道具，经验参数控制、法宝合成参数控制、法宝天赋技能参数控制）

│　 │ 　├ FabaoDesp.xml（宝物品和符箓物品属性显示控制）

│　 │ 　├ FabaoInlay.xml（法宝符箓对应物品属性控制）

│　 │ 　├ FabaoUpgrade.xml（法宝强化相关参数控制）

│　 │ 　├ WSPCfg.xml（万兽谱属性配置）

│　 │ 　├ Privilege.xml（最新中州英豪、神武天王特权配置）

│　 │ 　├ BOSSTJ.xml （BOSS图鉴系统配置）

│　 │ 　├ NewShop.xml （新版商城系统配置,可按需开启）

│　 │ 　└ TimeAchieve.xml （时光成就系统配置）

│　 │ 　├ JewelLevel.xml (符石等级套装属性配置)

│　 │ 　├ StarEquips.xml (装备升星系统配置)

│　 │ 　├ xunzhang_grow.csv(勋章系统)

│　 │ 　├ Shield.xml(盾牌系统)

│　 │ 　├ beast_attr.csv (灵枪区灵兽属性表)

│　 │ 　├ beast_fenghao.csv (灵枪区封号属性表)

│　 │ 　├ ride_grow.csv (灵枪区骑术等级属性表)

│　 │ 　├ yushoushi_grow.csv (灵枪区御兽师属性表)

│　 │ 　├ xiuluodengji_grow.csv(修罗等级属性表)

│　 │ 　├ xiuluoxinfa_grow.csv(修罗心法属性表)

│　 │ 　├ touxiangkuang.csv (头像框功能) 

│　 │ 　├ AntiHookWords.txt (验证脱机语句配置文件)

│　 │ 　├ AntiHookMsgTemplate.txt (验证窗口模板配置文件)

│　 │ 　├ equip_recover.csv (装备回收配置文件)

│　 │ 　├ GameStage.xml (19周年时光“服务器阶段”界面配置文件)

│　 │ 　├ GameHelp.txt (帮助信息文本配置文件)

│　 │ 　├ mobing.csv (魔兵属性配置文件)

│　 │ 　├ mobing_taozhuang.csv (魔兵套装属性文件)

│　 │ 　├ Xwl.xml (玄武炉配置文件)

│　 │ 　└ Slzh.xml(神龙之魂系统相关配置)

│　 │

│　 ├ ConLog（人物登录日志目录）

│ 　│

│　 ├ Envir （游戏配置目录） 

│ 　│ 　├ MapQuest_def

│ 　│ 　│　└ QManage.txt（登陆脚本）--> 查看说明 

│　 │　 │ 

│　 │ 　├ Market_Def （交易NPC脚本目录）

│　 │ 　│　├ QFunction-0.txt（功能脚本）--> 查看说明

│　 │ 　│　├ QGuildTower-0.txt（行会通灵塔）--> 查看说明

│　 │ 　│　├ QWolShop-0.txt（商城功能）--> 查看说明

│　 │ 　│　└ QActivity-0.txt（活动大厅配置）

│　 │　 │ 

│　 │　 ├ Market_prices(交易NPC商品物价缓存) 

│　 │　 │ 

│ 　│　 ├ MonItems （怪物爆物品配置文件目录）

│ 　│ 　├ Npc_def （管理NPC脚本目录）

│ 　│　 ├ Task （任务目录）

│ 　│　 ├ QuestDiary（脚本和功能目录）

│ 　│ 　├ Robot_def（机器人目录）

│ 　│ 　├ MapQuest.txt（杀怪任务列表）

│　 │ 　├ AdminList.txt （GM管理员列表）--> 查看说明

│　 │ 　├ Answer.txt （问答题目列表）

│ 　│ 　├ DenyAccountList.txt （禁止登录帐号列表）

│ 　│ 　├ DenyChrNameList.txt （禁止登录角色列表）

│　 │ 　├ DenyIPAddrList.txt （禁止登录IP列表）

│　 │　 ├ DisableMakeItem.txt （禁止制造物品列表）

│ 　│ 　├ DisableMoveMap.txt （禁止用命令移动地图列表）

│ 　│ 　├ DisableSendMsgList.txt （禁止发言列表）

│　 │ 　├ DisableTakeOffList.txt （禁止取下物品列表）

│　 │ 　├ EnableMakeItem.txt （允许制造物品列表）

│　 │ 　├ GameLogItemNameList.txt （游戏日志过滤列表）

│ 　│ 　├ GuardList.txt （守卫分布配置文件） --> 查看说明

│　 │ 　├ ItemBindAccount.txt （物品绑定帐号列表）

│　 │　 ├ ItemBindChrName.txt （物品绑定角色列表）

│ 　│ 　├ ItemBindIPaddr.txt （物品绑定IP列表）

│ 　│ 　├ ItemNameList.txt （物品名字列表） 

│ 　│ 　├ MakeItem.txt （NPC炼制物品配置文件）

│ 　│ 　├ MapInfo.txt （游戏地图配置文件）--> 查看说明

│ 　│ 　├ Merchant.txt （交易NPC配置文件）--> 查看说明

│ 　│ 　├ MiniMap.txt （游戏小图配置文件）--> 查看说明

│ 　│ 　├ MonDropLimitList.txt （怪物爆物品限制列表）

│ 　│ 　├ Mongen.txt （刷怪配置文件）--> 查看说明

│ 　│ 　├ MonLifeSpan.txt （怪物寿命列表）

│ 　│ 　├ PlantPoint.txt （植树列表）--> 查看说明 

│ 　│ 　├ NoClearMonList.txt （禁止清除怪物列表）

│ 　│　 ├ Npcs.txt （管理NPC配置文件）

│　 │ 　├ StartPoint.txt （新人登录点,安全区配置文件）--> 查看说明

│　 │ 　├ UnbindList.txt （捆装物品解包配置文件）

│ 　│ 　├ UnForceMaster.txt （强行出师记录文件）

│ 　│ 　├ UnMaster.txt （正常出师记录文件）

│ 　│ 　├ UnMarry.txt （强行离婚记录文件）

│ 　│ 　├ Task.txt （任务列表文件）

│ 　│ 　├ MapEvent.txt（地图触发配置）

│ 　│ 　├ NpcName.txt（NPC名字,appr配置）

│ 　│ 　├ UserCmd.txt（自定义命令）

│ 　│　 ├ WolShop.txt（传世商城配置）

│　 │　 ├ SuiteItemsList.txt（套装配置）

│　 │　 ├ MonsterChild.txt (怪物召唤属下的配置文件，如：幽灵虫母、蚁巢等)

│　 │　 └ Robot.txt（系统机器人）

│ 　│

│ 　├ GuildDir （行会和宗族目录） 

│ 　│　 ├ Guilds （行会目录）

│　 │　 ├ Guildlist.txt （行会列表文件）

│ 　│ 　├ Clans （宗族目录） 

│ 　│ 　└ ClanList.txt （宗族列表文件） 

│ 　│

│ 　├ Map（服务器地图文件所在目录）

│ 　│

│　 ├ Notice（游戏公告文件所在目录）

│ 　│　├ BannerNotice.txt（游戏内6格上公告设置文件）

│ 　│　├ LineNotice.txt（游戏内聊天框公告设置文件）

│ 　│　└ Notice.txt（游戏登陆前设置文件） 

│ 　│

│ 　├ Log（引擎日志目录）

│ 　│

│　 ├ Share

│　 │

│ 　├ ShareV

│ 　│

│ 　├ !abuse.txt 

│　 ├ !runaddr.txt 

│ 　├ !servertable.txt

│ 　├ !setup.txt（引擎设置参数保存文件）

│ 　├ WolServer.exe（游戏引擎服务器程序）

│ 　├ qqwry.dat （纯真ip数据库）

│ 　├ MsgList.txt（在线发消息保存文件）

│ 　└ PlugList.txt（插件配置文件） 

│ 

├ RunGate（游戏网关目录）

│ 　├ RunGate.exe （游戏网关程序）

│ 　└ RunGate.ini （游戏网关配置文件）

│


├ SelGate（角色服务器目录）

│　├ BlockIPList.txt （角色选择网关IP过滤配置文件）

│　├ Config.ini （角色选择网关配置文件）

│　└ SelGate.exe （角色服务器程序）

│ 

├ LoginGate（登陆服务器目录） 

│　├ LoginGate.exe （登陆服务器程序） 

│　├ Config.txt （登陆网关配置文件）

│　├ BlockIPList 

│　└ BlockIPAreaLis

│ 
└ GameCenter.exe （游戏控制器） 

├ Config.ini（游戏控制器配置文件） 

└ TaskList.txt（智能开区任务配置文件）
