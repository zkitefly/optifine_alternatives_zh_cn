# OptiFine 替代品

页面原文：[https://lambdaurora.dev/optifine_alternatives](https://lambdaurora.dev/optifine_alternatives)

本文翻译来自 `WhitePaper233/optifine_alternatives_zh_cn`

## 为什么需要替代 OptiFine？

OptiFine最初是一个伟大的MOD, 最开始时它为玩家提供了许多游戏的优化。然而，随着时间的推移，它带来的好处越来越少，并给MOD作者们带来了许多问题。这是因为Minecraft的代码库多年来一直在改进，而OptiFine时常替换掉整段Minecraft 的代码，同时又是闭源的，因此很难弄清楚为什么OptiFine会与另一个作者制作的MOD不兼容。
另外值得注意的是，OptiFine本身并不支持Fabric，而且OptiFabric是很难维护的。

在现在的Minecraft时代，在Fabric的社区努力下，MOD作者们已经开始为OptiFine的大部分功能创建替代品，让玩家保持更好的性能，更好的MOD兼容性，以及更好的支持。

[OptiFabric：一篇关于1.16崩溃的笔记 (OptiFabric: A note about the 1.16 crashes)][optifabric_issue]

[optifabric_issue]: https://github.com/modmuss50/OptiFabric/issues/242

## 替代品列表

这个列表将列出我（LambdAurora）推荐的OptiFine替代品，所以对被列入的MOD有一些要求。

 - 它们必须是公开的——如果它们仅仅通过您向别人索要才能获得，则不符合条件
 - 必须遵守Mojang的EULA（用户协议）
 - PVP客户端（Badlion、Lunar等）和挂端不被视为MOD
 - 不得涉及挂端
 - 以某种方式改变游戏方式（如缩放）的MOD，如果有办法让服务器得以禁用它们，将得到优先推荐
 - 免费和开源的MOD将得到优先推荐

这个列表现在有一个漂亮的URL：https://lambdaurora.dev/optifine_alternatives
（中文版地址: https://whitepaper233.top）

### 贡献

你可以在`data`分支上通过 [GitHub](https://github.com/LambdAurora/optifine_alternatives) 提交拉动请求，为这个列表做出贡献。

## 替代品

### 性能优化

#### 客户端

- [Cull Leaves] - 对树叶方块进行剔除, 提供相较于原版巨大的性能提升。 类似于OptiFine的智能树叶特性。
  - 可用于：quilt: 1.17 -> 1.19, fabric: 1.16 -> 1.19  
- [Cull Particles] - 不渲染看不到的颗粒，不需要用钠（Sodium）。 
  - 可用于：fabric,quilt: 1.15 -> 1.19
- [Dynamic FPS] - 改善Minecraft在后台时的性能。 
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.14 -> 1.19
- [Enhanced Block Entities] - 用方块渲染实体，从而减少FPS降低，以及用支持资源包对其进行定制。
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.19
- [EntityCulling] - 使用异步路径跟踪来隐藏不可见的（方块）实体。
  - 可用于：fabric,quilt: 1.16 -> 1.19, forge: 1.8.9, forge: 1.16 -> 1.19
- [Sodium] - Minecraft的现代渲染引擎和客户端优化MOD。
  - 可用于：fabric,quilt: 1.16 -> 1.19

#### 一般

- [LazyDFU] - 使得DataFixerUpper的初始化变得"懒惰"。DataFixerUpper（简称DFU）是Minecraft用来将旧世界转换为你正在运行的当前版本的系统，在原版中，它在启动时被初始化，速度很慢（而且吃了很多资源）。这个MOD延迟了DFU的初始化，只在需要的时候初始化，例如，如果你只在多人游戏中玩，那么它永远不会被初始化。 
  - 可用于：fabric,quilt: 1.14 -> 1.19, forge: 1.16 -> 1.19  
- [Lithium] - 超强的游戏逻辑/服务器优化MOD。 
  - 可用于：fabric,quilt: 1.15 -> 1.19  
- [Phosphor] - 超强的照明引擎优化MOD。与Starlight不兼容。 
  - 可用于：fabric,quilt: 1.15 -> 1.19  
- [Starlight] - 重写光照引擎以修复灯光照性能和光照错误。使用自定义格式进行灯光存储。与Phosphor不兼容。 
  - 可用于：fabric,quilt,forge: 1.17 -> 1.19  

### 美化

- [Animatica] - 一个实现OptiFine/MCPatcher动画纹理格式的MOD。 
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.17 -> 1.19  
- [Chime] - 为更多的互动项目模型添加断言，用自定义格式的CIT替换。
  - 可用于：fabric: 1.16, fabric,quilt: 1.18 -> 1.19  
- [CIT Resewn] - 重新实现了MCPatcher的CIT（来自Optifine资源包的自定义物品纹理）。 
  - 可用于：fabric,quilt: 1.17 -> 1.19  
- [Clear Skies] - 使得地平线和雾与天空的颜色相匹配。真正的蓝天!  
  - 可用于：fabric,quilt: 1.15 -> 1.19, forge: 1.16  
- [Colormatic] - Minecraft的自定义颜色的MOD的独立实现。 
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.14 -> 1.19  
- [Connected Block Textures] - MCPatcher/Optifine连接纹理格式在Fabric上的实现。不维护。 
  - 可用于：fabric: 1.16  
  - 需要 [Fabric Renderer API](#compatibility "更多信息")  
- [Continuity] - 一个高效的支持连接纹理的Fabric MOD。支持发光纹理。 
  - 可用于：fabric,quilt: 1.17 -> 1.19  
  - 需要 [Fabric Renderer API](#compatibility "更多信息")  
- [Custom Entity Models (CEM)] - 一个主要基于Optifine格式的自定义实体模型的实现，旨在实现与Optifine相同的自定义实体模型的功能。 
  - 可用于：fabric,quilt: 1.16 -> 1.19  
- [Custom GUI] - 一个允许对GUI纹理进行动画处理或用最小断言替换容器纹理的MOD。 
  - 可用于：fabric: 1.16 -> 1.17  
- [Entity Texture Features] - 一个Fabric MOD，为资源包实现了对生物的随机和发光纹理支持。与Optifine格式兼容且与Sodium兼容。 
  - 可用于：quilt: 1.18 -> 1.19, fabric,forge: 1.16 -> 1.19  
- [FabricSkyboxes] - 允许资源包自定义天空盒。OptiFine格式默认是不兼容的，但有转换器可用。 
  - 可用于：fabric,quilt: 1.16 -> 1.19  
- [JMX] - JMX为Minecraft JSON模型加载增加了对FREX渲染接口的支持。它也可以被配置为将所有JSON模型加载为FREX网格，由于更有效的数据结构，这可能会适度减少内存使用。 
  - 可用于：fabric,quilt: 1.16 -> 1.19  
- [JsonEM (Json Entity Models)] - 数据驱动的实体模型库，理论可用于大多数实体。不支持OptiFine的格式。 
  - 可用于：quilt,fabric: 1.18 -> 1.19  
- [LambdaBetterGrass] - 为游戏添加更好的草和雪。 
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.19  
  - 需要 [Fabric Renderer API](#compatibility "更多信息")  
- [LambDynamicLights] - 在游戏中添加动态光源。 
  - 可用于：quilt: 1.17 -> 1.19, fabric: 1.15 -> 1.19  
- [More Block Predicates] - 允许资源包根据新的条件改变方块模型，自定义的格式。 
  - 可用于：fabric,quilt: 1.17 -> 1.19  
- [MoreMcmeta] - 用更多的选项将几乎任何Minecraft纹理制作成动画。 
  - 可用于：fabric,quilt: 1.16 -> 1.19, forge: 1.16 -> 1.19  
- [Transparent] - 允许资源包使实体支持透明度。 
  - 可用于：fabric,quilt,forge: 1.15 -> 1.19  
- [Varied Mob Textures] - 此MOD允许资源包创建者为同一个生物提供多个随机纹理。使用自定义格式，基于OptiFine的资源包需要转换。 
  - 可用于：fabric: 1.16  

#### 过场页面

- [Custom Splash Screen] - 根据你的喜好改变Minecraft的加载屏幕! 完全可配置!  
  - 可用于：quilt: 1.18, fabric: 1.16 -> 1.18  
- [Dark Loading Screen] - 一个简单的MOD，使加载屏幕变为暗黑模式。 
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.15 -> 1.19  
- [Quilt Loading Screen] - 一个基于The Quilt Community的服务器横幅的加载屏幕。 
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.18  
- [Splash] - Splash是一个允许你定制你的过场页面颜色的Fabric MOD。 
  - 可用于：fabric: 1.16 -> 1.17  

### 着色器

- [Canvas Renderer] - 一个新的渲染引擎。与Sodium不兼容。 
  - 可用于：fabric,quilt: 1.17 -> 1.19, fabric: 1.16  
- [Iris] - Minecraft的一个新的着色器MOD，旨在与现有的着色器MOD/Optifine着色器兼容。 
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.19  

### 迷雾

- [ClearView] - 控制显示哪些种类的迷雾。 
  - 可用于：fabric: 1.15 -> 1.16  
- [Custom Fog] - 一个允许你自定义你的世界中的雾的外观的MOD。 
  - 可用于：fabric,quilt: 1.15 -> 1.18  
- [Fog Control] - 允许用户调整迷雾渲染的（客户端）距离，或完全禁用迷雾。  
  - 可用于：fabric: 1.17  
- [FogYeet] - 1.15的小MOD，用于去除迷雾。
  - 可用于：fabric: 1.15  
- [NoFog] - 一个简单的客户端MOD，同时支持Forge和Fabric，可以消除所有的雾气。 (ARR)  
  - 可用于：fabric,quilt: 1.16 -> 1.19, forge: 1.10.2 -> 1.19  

### 实用向

- [Fabrishot] - 拍摄分辨率高得惊人的屏幕截图，为什么不呢？ 
  - 可用于：fabric,quilt: 1.16 -> 1.19  
- [Resolution Control] - 允许你设置渲染分辨率和以高分辨率截图。 
  - 可用于：fabric: 1.14 -> 1.16  
- [ResolutionControl+] - 允许你设置渲染分辨率和以高分辨率截图。 
  - 可用于：fabric: 1.16 -> 1.17, fabric: 1.19  

#### 云层高度

- [Raised Clouds] - 允许改变云层高度。 
  - 可用于：fabric,quilt: 1.16 -> 1.19  
- [Soaring Clouds] - 允许改变云层高度。 
  - 可用于：fabric: 1.15 -> 1.16  

#### 缩放

- [Camera Utils] - 关于玩家视角的额外功能。 
  - 可用于：fabric,quilt: 1.17 -> 1.19  
- [Logical Zoom] - 用于Minecraft的超级简单的缩放键。 
  - 可用于：fabric,quilt: 1.15 -> 1.19  
- [Ok Zoomer] - 为Fabric增加了一个高度可配置的缩放键。为你定制的缩放!  
  - 可用于：quilt: 1.18 -> 1.19, fabric: 1.14 -> 1.18  
- [Quick Spyglasser] - 为使用物品栏中任何地方的望远镜增加了一个客户端按键。 
  - 可用于：fabric: 1.17  
- [Zoomify] - 一个相当简单的缩放MOD，具有适度的可定制性。 
  - 可用于：fabric,quilt: 1.18 -> 1.19  

[Cull Leaves]: https://modrinth.com/mod/cull-leaves "Cull Leaves Modrinth 页面"
[Cull Particles]: https://curseforge.com/minecraft/mc-mods/cull-particles-fabric "Cull Particles CurseForge 页面"
[Dynamic FPS]: https://modrinth.com/mod/dynamic-fps "Dynamic FPS Modrinth 页面"
[Enhanced Block Entities]: https://modrinth.com/mod/ebe "Enhanced Block Entities Modrinth 页面"
[EntityCulling]: https://modrinth.com/mod/entityculling "EntityCulling Modrinth 页面"
[Sodium]: https://modrinth.com/mod/sodium "Sodium Modrinth 页面"
[LazyDFU]: https://modrinth.com/mod/lazydfu "LazyDFU Modrinth 页面"
[Lithium]: https://modrinth.com/mod/lithium "Lithium Modrinth 页面"
[Phosphor]: https://modrinth.com/mod/phosphor "Phosphor Modrinth 页面"
[Starlight]: https://modrinth.com/mod/starlight "Starlight Modrinth 页面"
[Animatica]: https://modrinth.com/mod/animatica "Animatica Modrinth 页面"
[Chime]: https://modrinth.com/mod/chime "Chime Modrinth 页面"
[CIT Resewn]: https://modrinth.com/mod/cit-resewn "CIT Resewn Modrinth 页面"
[Clear Skies]: https://modrinth.com/mod/clear-skies "Clear Skies Modrinth 页面"
[Colormatic]: https://modrinth.com/mod/colormatic "Colormatic Modrinth 页面"
[Connected Block Textures]: https://github.com/TwilightFlower/connected-block-textures "Connected Block Textures GitHub 页面"
[Continuity]: https://modrinth.com/mod/continuity "Continuity Modrinth 页面"
[Custom Entity Models (CEM)]: https://modrinth.com/mod/cem "Custom Entity Models (CEM) Modrinth 页面"
[Custom GUI]: https://modrinth.com/mod/customgui "Custom GUI Modrinth 页面"
[Entity Texture Features]: https://modrinth.com/mod/entitytexturefeatures "Entity Texture Features Modrinth 页面"
[FabricSkyboxes]: https://modrinth.com/mod/fabricskyboxes "FabricSkyboxes Modrinth 页面"
[JMX]: https://modrinth.com/mod/imx "JMX Modrinth 页面"
[JsonEM (Json Entity Models)]: https://modrinth.com/mod/jsonem "JsonEM (Json Entity Models) Modrinth 页面"
[LambdaBetterGrass]: https://modrinth.com/mod/lambdabettergrass "LambdaBetterGrass Modrinth 页面"
[LambDynamicLights]: https://modrinth.com/mod/lambdynamiclights "LambDynamicLights Modrinth 页面"
[More Block Predicates]: https://modrinth.com/mod/mbp "More Block Predicates Modrinth 页面"
[MoreMcmeta]: https://modrinth.com/mod/moremcmeta "MoreMcmeta Modrinth 页面"
[Transparent]: https://modrinth.com/mod/transparent "Transparent Modrinth 页面"
[Varied Mob Textures]: https://curseforge.com/minecraft/mc-mods/varied-mob-textures "Varied Mob Textures CurseForge 页面"
[Custom Splash Screen]: https://modrinth.com/mod/custom-splash-screen "Custom Splash Screen Modrinth 页面"
[Dark Loading Screen]: https://curseforge.com/minecraft/mc-mods/dark-loading-screen "Dark Loading Screen CurseForge 页面"
[Quilt Loading Screen]: https://modrinth.com/mod/quilt-loading-screen "Quilt Loading Screen Modrinth 页面"
[Splash]: https://curseforge.com/minecraft/mc-mods/splash "Splash CurseForge 页面"
[Canvas Renderer]: https://modrinth.com/mod/canvas "Canvas Renderer Modrinth 页面"
[Iris]: https://modrinth.com/mod/iris "Iris Modrinth 页面"
[ClearView]: https://curseforge.com/minecraft/mc-mods/clearview "ClearView CurseForge 页面"
[Custom Fog]: https://modrinth.com/mod/custom-fog "Custom Fog Modrinth 页面"
[Fog Control]: https://modrinth.com/mod/fog-control "Fog Control Modrinth 页面"
[FogYeet]: https://modrinth.com/mod/fogyeet "FogYeet Modrinth 页面"
[NoFog]: https://modrinth.com/mod/no_fog "NoFog Modrinth 页面"
[Fabrishot]: https://modrinth.com/mod/fabrishot "Fabrishot Modrinth 页面"
[Resolution Control]: https://curseforge.com/minecraft/mc-mods/resolution-control "Resolution Control CurseForge 页面"
[ResolutionControl+]: https://modrinth.com/mod/resolution-control-plus "ResolutionControl+ Modrinth 页面"
[Raised Clouds]: https://curseforge.com/minecraft/mc-mods/raised-clouds "Raised Clouds CurseForge 页面"
[Soaring Clouds]: https://curseforge.com/minecraft/mc-mods/soaring-clouds "Soaring Clouds CurseForge 页面"
[Camera Utils]: https://modrinth.com/mod/camera-utils "Camera Utils Modrinth 页面"
[Logical Zoom]: https://modrinth.com/mod/logical-zoom "Logical Zoom Modrinth 页面"
[Ok Zoomer]: https://modrinth.com/mod/ok-zoomer "Ok Zoomer Modrinth 页面"
[Quick Spyglasser]: https://curseforge.com/minecraft/mc-mods/quick-spyglasser "Quick Spyglasser CurseForge 页面"
[Zoomify]: https://modrinth.com/mod/zoomify "Zoomify Modrinth 页面"


### 额外

下面列出的MOD不属于OptiFine的直接替代品，但这些MOD还是很好用的。

- [Ears] - 精美时尚的fuzzy folk特性，它提供了大量的皮肤定制选项，直接编码到上传到Mojang的皮肤文件中。比起限制性的披风，这是一个非常好的表达自己的选择。
  - 可用于：b1.7.3, 1.2.5, 1.4.7 -> 1.19, Not so Seecret Saturday (a1.1.2), New Frontier Craft (b1.7.3)
- [DashLoader] - 试图通过缓存游戏的内容来改善加载时间。可能与此列表中的一些MOD不兼容。
  - 可用于：1.16 -> 1.19
- [Entity View Distance] - 这种模式允许在客户端和服务器上更精确地操纵视距。 
  - 可用于：1.17 -> 1.19
- [FerriteCore] - 内存占用优化。 
  - 可用于：[1.16 -> 1.19][FerriteCore], [1.16 -> 1.19 (Forge)](https://www.curseforge.com/minecraft/mc-mods/ferritecore)
- [Hydrogen] - 在更多的模组使用场景中减少游戏的内存使用。 
  - 可用于：1.16 -> 1.17
- [Krypton] - 一个优化Minecraft网络栈的MOD。 
  - 可用于：1.16 -> 1.19
- [Overworld Two] 提供了一个替代的优化的世界的生成器，用于主世界和地狱。比原版快得多，但与原版不完全相同。
  - 可用于：1.16
- [Sodium Extra] - 增加了额外的没有在钠中出现的功能。
  - 可用于：1.16 -> 1.19
- [Reese's Sodium Options] - 新的钠的选项菜单界面，目的是改善用户体验。 
  - 可用于：1.16 -> 1.19

[Ears]: https://ears.unascribed.com/ "Ears 网站"
[FerriteCore]: https://modrinth.com/mod/ferrite-core "FerriteCore Modrinth 页面"
[Entity View Distance]: https://modrinth.com/mod/entity-view-distance "Entity View Distance Curseforge 页面"
[Hydrogen]: https://modrinth.com/mod/hydrogen "Hydrogen Modrinth 页面"
[Krypton]: https://modrinth.com/mod/krypton "Krypton Modrinth 页面"
[DashLoader]: https://modrinth.com/mod/dashloader "DashLoader Modrinth 页面"
[Overworld Two]: https://www.curseforge.com/minecraft/mc-mods/overworld-two "Overworld Two Curseforge 页面"
[Sodium Extra]: https://modrinth.com/mod/sodium-extra "Sodium Extra Modrinth 页面"
[Reese's Sodium Options]: https://modrinth.com/mod/reeses-sodium-options "Reese's Sodium Options Modrinth 页面"

### 非动态FOV

**从1.16.2及以上版本开始，这现在是无障碍设置下的一个普通功能。如果你在1.16.2或以上版本的游戏中，这个功能与MOD无关。**

这些都是客户专用的MOD，可以防止Minecraft在所有情况下改变FOV。

- [motioNO] - 禁用动态FOV。 
- [FovLock] - 增加了动态FOV锁定按钮。

[motioNO]: https://www.curseforge.com/minecraft/mc-mods/motiono "MotioNo CurseForge 页面"
[FovLock]: https://github.com/ChloeDawn/FovLock "FovLock GitHub 页面"

## 兼容性

Sodium和Canvas渲染器兼容。

一些MOD需要Fabric Renderer API才能工作，Canvas支持它，但Sodium默认不会支持它，需要安装 [Indium] 以添加对其的支持。

- [Indium] - 将对Fabric Renderer API的支持添加到 [Sodium](https://modrinth.com/mod/sodium).
  - 可用于：1.16 -> 1.19

[Indium]: https://modrinth.com/mod/indium "Indium Modrinth 页面"

## 缺失的

- 自定义实体模型（可能会在Vanilla中出现，但何时未知），目前还没有完全被取代：目前对原版实体修改的实现都是硬编码。 

## 需要帮助？

如果你需要关于钠、锂、磷（简称CaffeineMC的任何一个mod）的帮助，[请查看CaffeineMC的discord服务器](https://jellysquid.me/discord).

如果你需要与LambDynamicLights、LambdaBetterGrass或Inspecio相关的帮助，且你不想在评论中发表建议，你可以查看 [我自己的discord服务器](https://discord.lambdaurora.dev)

## 其他列表

 - [有用的Fabric服务器端MOD](https://github.com/comp500/fabric-serverside-mods/blob/main/README.md)

<script src="https://giscus.app/client.js"
        data-repo="zkitefly/zkitefly.github.io"
        data-repo-id="R_kgDOHnuxMQ"
        data-category="General"
        data-category-id="DIC_kwDOHnuxMc4CR1BS"
        data-mapping="pathname"
        data-strict="1"
        data-reactions-enabled="1"
        data-emit-metadata="1"
        data-input-position="top"
        data-theme="preferred_color_scheme"
        data-lang="zh-CN"
        data-loading="lazy"
        crossorigin="anonymous"
        async>
</script>
