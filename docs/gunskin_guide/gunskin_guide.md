# 皮肤资源包制作指南

## 开始之前
欢迎来到LesRaisins提供的tac皮肤资源包制作指南

### 请注意：  
1. 本指南不是皮肤本身的纹理绘制或模型制作的美术教程，而仅仅是帮助读者正确创作枪械模型/纹理、以及将已经制作好的皮肤纹理与模型实装进游戏的说明文档，同时，为了避免阅读障碍，也请确保在阅读本章节的内容掌握基础的资源包制作知识和相关概念； 
2. 本指南的部分页面与小节可能带有`legacy`标识，这代表这部分内容可能不适用于最新版的TaC，详情请参阅对应页面的说明  
3. 本指南中许多示例内容的具体文件都包含在TaC本体的资产文件夹中，如果你觉得本指南描述的不够直观，不妨直接打开源文件看看，也许有助于理解

## 一些说明
### 关于模型
在游戏中tac最终呈现的枪械的`完整的模型`是由一系列来自不同文件的模型组合而来的；  

对于这一系列模型，我们在本指南中其称之为`模型部件`或者`部件`；  


## 制作一个枪械皮肤
关于如何正确获取原始素材和开始绘制皮肤，请参阅 [章节：皮肤绘制帮助](./gunskin_guide/paint.md)

## 描述文件格式
要让模组读取资源包里的枪械皮肤，你需要在资源包里添加一个json文件以描述皮肤  
具体的路径为
`assets/<命名空间>/models/gunskin/skin.json`  
你可以这个文件放到任意一个命名空间的对应路径下，这会决定你接下来皮肤的命名空间。（其中，TaC 的`<命名空间>`为`tac`）

关于`描述文件`的详细内容，请参阅 [章节：描述文件格式](./gunskin_guide/description_file.md)


## 调用皮肤
贼简单,`/give @s tac:ak47{Skin:"<皮肤命名空间>:<皮肤标识符>"}`,可以不加命名空间,默认是`tac`,
比如有一把ak的皮肤,`skin.json`放在`tac`的命名空间里,比如上例中的黄金和白银ak,
就是`/give @s tac:ak47{Skin:"golden"}` `/give @s tac:ak47{Skin:"tac:silver"}`  
