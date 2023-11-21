# Unity实例：走迷宫找到出口
> 日期：2023年11月21日
> 班级：数字媒体技术1302班
> 课程：游戏应用程序开发
> 环境：Unity 2022.3.9f1c1

# 开发准备
## 核心功能
1. 创建主角
2. 

## 资源准备
1. 去 [Unity Assets Store](https://assetstore.unity.com/) 下载官方资源：[3D Beginner](https://assetstore.unity.com/packages/essentials/tutorial-projects/unity-learn-3d-beginner-tutorial-resources-urp-143848)
2. 检查资源兼容性，URP通用渲染管线和SRP可编程渲染管线


# 开发过程

## 项目创建
1. 查看版本是否支持某些3D模板
2. 选择普通`3D(URP)`模板，创建项目`INS01_3DTutorial`
3. 下载Package之后，开始开发程序

## 场景搭建
1. 在Store界面点击`添加到我的资源`，选择`在Unity中打开`
2. 然后在`Package Manager`选择`Download`，等待下载完成
3. 选择`Import --> Next`，等待资源导入
4. 在`UnityTechnologies\Prefebs`将官方下载的Package中的Prefeb预制体场景`Level`拖出来
5. 给场景的 Position Reset一下。
6. 给Scene更名为`MainScene`，方便后续开发

## 添加角色
1. 在该路径下：`Models\Characters`
2. 将 `JohnLemon` 的 `Prefeb` 拖到场景 (MainScene) 中并 `Reset Position`

## 角色动画 Animator
1. 形成动画的方式：修改Transform的属性
2. 使用Unity的动画资源
   1. 在Animation\Animation下找到John@Walk和John@Idle
3. 创建动画
   1. Window --> Animation 打开Animation窗口
   2. 新建一个动画，查看Inspector面板，可以看到Animator
   3. 在Animator窗口，可以看到John连接到了TestAnimation
   4. 删除TestAnimation，将Unity中的John@Idle导入进来并让John连接到Idle动画
   5. 点击运行游戏，可以查看到效果。
4. Animation 和 Animator 的区别

| Animation | Animator |
| ---- | ---- |
| 动画设置，设置某个动画的关键帧 | 动画控制器：动画切换、叠加 |