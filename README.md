# UniversalUnityDemosaics
BepInEx插件的集合，用于Unity3D引擎中的游戏，用于消除马赛克审查。他们主要针对日本3D游戏（无尽的游戏）。他们也可以玩一些2D游戏。大多数插件需要最新版本的BepInEx 5。

你可以在这里看到一些由这些插件去马赛克的游戏示例。

### BepInEx插件的集合，用于Unity3D引擎中的游戏，用于消除马赛克审查。他们主要针对日本3D游戏（无尽的游戏）。他们也可以玩一些2D游戏。大多数插件需要最新版本的BepInEx 5。

你可以在这里看到一些由这些插件去马赛克的游戏示例。

### DumbRenderer演示
基本的“面包和黄油”演示。它适用于最大数量的游戏和应该是第一个尝试。它的工作原理是禁用离散马赛克对象和删除其纹理。

### DumbRenderDemosaicIl 2Cpp的
一个为IL2CPP游戏制作的DumbRendererDemosit版本。IL2CPP需要最新版本的BepInEx 6。

### 组合网格演示
一个更智能的DumbRendererDemocrat版本，适用于使用较新的Unity版本中提供的组合网格渲染器的游戏（DumbRendererDemocrat根本不适用于这些游戏）。扫描所有渲染器上的单个材质，以查找可能是马赛克的材质，并将其着色器更改为不可见。当网格被组合而不是由变换表示时有用。如果有任何专用的马赛克渲染器，请与DumbRendererDemo一起使用。

### 材料替换演示
一个更聪明的版本DumbRendererDemocrat，取消审查一些Live2D游戏，其中私人完全消失与其他democrat插件。

### 着色器替换演示
扫描所有渲染器上材质的单个着色器，以查找可能是马赛克的着色器，并将其替换为指定的着色器。当马赛克效果是通过在完全建模的网格上使用自定义着色器来实现时很有用。确保设置“替换着色器名称”设置！您可以在ConfigurationManager中更改设置，更改将立即应用。您可以使用RuntimeUnityEditor找出不同渲染器上的着色器的名称，只需找到所需的渲染器，检查它，然后查看sharedMaterial ->着色器内部。如果有任何专用的mozaic渲染器，请与DumbRendererDemo一起使用。

### DumbTypeDemosaic的
DumbRendererDemocracy的一个变体，用于检查游戏代码中可能的马赛克方法并禁用它们。它很少工作，但需要一些游戏。

### CubismRenderer禁用演示
使用CubismModel框架针对游戏的Demo。通常DumbRendererDemosaic已经足够好了，但有些游戏可能会更好地使用这个。

### 如何使用？
获取最新版本的BepInEx 5（对于IL2CPP版本获取此版本）并将其安装到您的游戏中。
将其中一个democracy.dll文件复制到BepInEx\plugins文件夹。
看看插件加载和对游戏有没有影响。如果没有，请删除它并尝试另一个。
